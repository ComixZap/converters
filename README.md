# Converter scripts

These scripts are designed to convert .cbr or .pdf files to the .cbz format,
which has better support.

## filecheck

Checks to make sure zip-compatible files are named `.cbz`, and rar-compatible
files are named `.cbr`. This should be run when adding new files to a
collection, before running `cbrtocbz`.

### Usage

```shell
./filecheck collection-root-directory
```

## cbrtocbz

Converts .cbr files to .cbz files. Other files are ignored. Requires the
following utilities:
* 7z
* unrar
* zip

### Usage

```shell
./cbrtocbz collection-root-directory
```

## pdftocbz

Converts .pdf files to .cbz files. Other files are ignored. Requires the
following utilities:
* pdfimages
* zip

### Usage

```shell
./pdftocbz collection-root-directory
```
