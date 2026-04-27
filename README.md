# Assignment 1 – Circular Buffer Implementation (C Language)

## Overview
This project implements a simple Circular Buffer in the C programming language.  
The buffer supports the following operations:

- Initialization  
- Writing data (enqueue)  
- Reading data (dequeue)  
- Detecting buffer full and empty states  

The implementation uses manual pointer movement (head, tail) and modular arithmetic to achieve circular behavior.

---

## How the Circular Buffer Works
The buffer is represented using:

- `buffer[]` : Array that stores characters  
- `head` : Index used for reading  
- `tail` : Index used for writing  
- `count` : Number of stored elements  

The buffer is:

- Empty when `count == 0`  
- Full when `count == SIZE`  

Pointer movement uses:
(index + 1) % SIZE

This ensures circular wrapping.

---

## Implemented Functions

### 1. Initialization
Resets head, tail, and count to zero.

### 2. isFull()
Returns true when the buffer is full.

### 3. isEmpty()
Returns true when the buffer is empty.

### 4. writeBuffer()
Writes a character into the buffer if space is available.  
Handles overflow by printing a warning.

### 5. readBuffer()
Reads a character from the buffer if not empty.  
Handles underflow by printing a warning.

---

## Program Flow (main)
1. The program asks the user to enter their name.  
2. The string `"CE-ESY"` is appended to the entered name.  
3. Each character is written into the circular buffer.  
4. The program reads all characters back from the buffer.  
5. The final output is printed on the screen.  
6. The buffer becomes empty after reading all characters.

---

## How to Compile and Run

### Using GCC:
gcc prog.c -o program
./program

### Or using an online compiler:
Programiz Online C Compiler can be used to run the code.

---

## Notes
- You can change the buffer size (`SIZE`) to test overflow and normal behavior.  
- The implementation avoids using any built‑in data structures.  
- The code follows clean coding practices and clear function separation.

---

## Repository Structure
Assignment1/
│
├── prog.c
└── README.md



## Author
Aya – CE‑ESY26
