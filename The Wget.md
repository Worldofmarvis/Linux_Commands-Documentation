Wget (Web Get)

Wget is a free utility for non-interactive downloading of files from the web. It supports HTTP, HTTPS, and FTP protocols, as well as retrieval through HTTP proxies. Wget is designed for robustness over slow or unstable network connections, and can continue interrupted downloads.

A key feature is its ability to download recursively, following links to mirror entire websites or directory structures.

Wget is commonly used for:

-Automating file downloads in scripts
-Mirroring or backing up websites
-Downloading files on servers or systems without a graphical interface

Wget Command Format

-wget [options] [URL]

Common Examples:

  -wget https://example.com/file.zip`
  -wget -r -l 5 https://example.com/` (recursively download up to 5 levels deep)
  -wget -P /path/to/save https://example.com/file.iso` (download to a specific directory)
  -wget -O custom_name.deb https://example.com/package.deb` (download and save with a different filename)