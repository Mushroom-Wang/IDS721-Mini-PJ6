# Rust File Compression Tool
This project is a simple command-line tool for compressing files using the Gzip compression algorithm. The tool is written in Rust and uses the `flate2` crate to perform the compression.

## Installation
To use this tool, you will need to have Rust installed on your system. You can install Rust by following the instructions on the official Rust website.

Once Rust is installed, you can download this project by cloning the repository:
```
git clone https://github.com/Mushroom-Wang/IDS721-Mini-PJ6
```

## Usage
To use the tool, simply run the `compress_file` executable with two arguments: the path to the source file and the path to the target file. For example:
```
cargo run rust.pdf compressed_file
```

## How it works
The tool works by opening the source file using a BufReader, creating a Gzip encoder using the GzEncoder struct from the flate2 crate, and then copying the contents of the source file to the encoder. The compressed data is then written to the target file.

The tool also prints some basic information about the size of the source and target files, as well as the amount of time it took to compress the file.

## References

* [rust-cli-template](https://github.com/kbknapp/rust-cli-template)
