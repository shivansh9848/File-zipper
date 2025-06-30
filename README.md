# File-zipper

A File zipper project based on Huffman Coding, a lossless, bottom-up compression algorithm. It can compress and decompress any text files.

## How to Run

### Compilation

First, compile the encoder and decoder programs:

```cmd
g++ -o encode.exe encode.cpp huffman.cpp
g++ -o decode.exe decode.cpp huffman.cpp
```

### Usage

**To compress a file:**

```cmd
encode.exe <input_file> <compressed_output_file>
```

Example:

```cmd
encode.exe inputFile.txt compressed.huf
```

**To decompress a file:**

```cmd
decode.exe <compressed_file> <decompressed_output_file>
```

Example:

```cmd
decode.exe compressed.huf decompressed.txt
```

### Example Workflow

1. Compile both programs using the commands above
2. Compress a text file: `encode.exe inputFile.txt compressed.huf`
3. Decompress the file: `decode.exe compressed.huf decompressed.txt`
4. Compare the original and decompressed files to verify they are identical

## Files

- `huffman.hpp` & `huffman.cpp` - Core Huffman coding implementation
- `encode.cpp` - Compression program
- `decode.cpp` - Decompression program
- `inputFile.txt` - Sample input file for testing
- `compressed.huf` - Compressed output file (generated after encoding)
- `decompressed.txt` - Decompressed output file (generated after decoding)
