The `binwalk` Command

`binwalk` is a tool for analyzing, reverse engineering, and extracting firmware images and other binary files. It scans a file for embedded files, signatures, and known file-type headers hidden inside a larger blob of data.

`binwalk` is especially useful in CTFs where flags or files are hidden inside images, firmware dumps, or other binaries through steganography or embedding.

`binwalk` is commonly used for:

- Identifying embedded files (images, archives, executables) inside a binary
- Extracting hidden or appended data from files
- Analyzing firmware for reverse engineering

## binwalk Command Format

```
binwalk -e suspicious_file.bin
```

## Common Flags

- `-e` — extract any files identified inside the target
- `-M` — recursively scan extracted files (matryoshka mode)
- `-B` — scan target for common file signatures (default behavior)
- `--dd='.*'` — extract all identified signatures, regardless of type

## CTF Example

Given an image file (`flag.png`) that looks normal but is larger than expected:

```
binwalk -e flag.png
```

This can reveal a ZIP archive, embedded text, or another file appended after the PNG's end marker — a common technique for hiding CTF flags inside images.
