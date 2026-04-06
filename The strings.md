**Strings**

The `strings` command is a utility found in most Unix-like operating systems (Linux, macOS, BSD) and also available on Windows via tools like Cygwin or WSL. It extracts and displays sequences of printable characters (strings) from binary files. This is especially useful for examining non-text files such as executables, object files, libraries, or raw data dumps, where human-readable content (like error messages, variable names, or embedded text) is often buried inside machine code.

By default, `strings` looks for sequences of 4 or more consecutive printable characters (adjustable with the `-n` option). It works by scanning the binary data, filtering out non-printable bytes, and outputting the resulting text to standard output.

`strings` is commonly used for:

-   **Reverse engineering** – Finding embedded clues, function names, or strings inside compiled binaries.
-   **Forensics & malware analysis** – Extracting readable text from suspicious executables or memory dumps.
-   **Debugging** – Checking what text a library or program contains without having source code.
-   **Data recovery** – Pulling plaintext fragments from corrupted files or raw disk images.

**Strings Command Format**

`strings [options] [file(s)]`

**Common Examples:**

-   `strings /bin/ls` – Show all printable strings in the `ls` binary.
-   `strings -n 8 myprogram.exe` – Only show strings at least 8 characters long.
-   `strings -t d image.bin` – Show strings with their decimal offset positions within the file.
-   `strings -n 10 -f *.so` – Scan all `.so` shared libraries, prefixing each string with the filename.
-   `strings -e l /proc/self/exe` – Use 16‑bit little‑endian encoding (useful for Unicode or UTF‑16 text).
