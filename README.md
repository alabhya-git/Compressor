# File Compression System

This is a Java-based file compression and decompression tool I made using Huffman encoding. It supports both compression and decompression of files through a simple GUI built with Swing. The algorithm is lossless and uses prefix codes to reduce file size efficiently.

## Features

- Compresses and decompresses files using Huffman coding
- GUI with file chooser and progress bar
- Custom implementations of linked lists and priority queue
- Threaded text display for better UI responsiveness

## Project Structure

src/
├── CharLinkedList.java
├── HuffmanTree.java
├── HuffmanEncoder.java
├── HuffCompression.java
├── EncoderGUI.java
├── ProgressBar.java
├── Message.java
├── QueueLL.java
├── ThreadedText.java
├── Displayer.java
└── various node/structure classes like ByteNode, Node, CharNode

## Prerequisites

- Java 8 or higher
- Optional: Maven for building (project includes a pom.xml)
- Java IDE like IntelliJ or Eclipse, or command line tools

## Installation and Running

1. Clone the repository:

   git clone https://github.com/ammarlodhi255/file-compression-system.git
   cd file-compression-system

2. Build the project:
   - If you're using Maven:
     mvn clean package
   - Or just open it in an IDE and run the source files

3. Run the GUI:
   - In IDE: Run `EncoderGUI.java`
   - Or from terminal:
     java -cp target/classes EncoderGUI

## Usage

- Click "Choose File" to select a file for compression
- Click "Compress" to save the .huf file
- Click "Decompress" and select a .huf file to restore the original file

## How it works

The encoder reads the file and counts character frequencies. A Huffman tree is constructed using a custom priority queue, and prefix codes are generated. The file is then encoded and saved along with header metadata so it can be decompressed back later.
