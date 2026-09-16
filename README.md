# Playfair Cipher – Virtual Lab

## Experiment Name
**Playfair Cipher Encryption and Decryption**

## Aim
To understand and implement the Playfair Cipher for encryption and decryption by generating a 5×5 key square from a user-provided keyword and processing messages as pairs of letters.

---

## Objectives

- Generate a 5×5 Playfair key square from a user-provided key.
- Handle duplicate letters and the I/J combination.
- Prepare plaintext into digraphs (pairs of letters).
- Encrypt messages using the Playfair Cipher rules.
- Decrypt ciphertext using the reverse Playfair Cipher rules.
- Visualize the encryption/decryption process step-by-step.
- Test the understanding of the Playfair Cipher using an interactive quiz.

---

## About the Playfair Cipher

The Playfair Cipher is a classical symmetric encryption technique that encrypts **pairs of letters (digraphs)** instead of individual letters.

A keyword is used to construct a **5×5 key square** containing 25 letters. Since the English alphabet contains 26 letters, **I and J share one cell**.

The cipher uses three main rules:

1. **Same Row**  
   Each letter is replaced by the letter immediately to its right. Wrapping is applied at the end of the row.

2. **Same Column**  
   Each letter is replaced by the letter immediately below it. Wrapping is applied at the bottom of the column.

3. **Rectangle Rule**  
   If the two letters are in different rows and columns, each letter is replaced by the letter in its own row and the other letter's column.

For decryption, the row and column shifts are reversed.

---

## Features

### 1. Key Square Generation
- Accepts a user-provided keyword.
- Removes duplicate characters.
- Converts `J` to `I`.
- Automatically fills the remaining alphabet characters.
- Generates a 5×5 key square dynamically.

### 2. Encryption
- Accepts plaintext from the user.
- Removes spaces and non-alphabetic characters.
- Converts `J` to `I`.
- Splits plaintext into digraphs.
- Inserts `X` between repeated letters.
- Adds `X` if the message has an odd number of characters.
- Generates the corresponding ciphertext.

### 3. Decryption
- Accepts ciphertext from the user.
- Processes the ciphertext as letter pairs.
- Applies the reverse Playfair rules.
- Displays the recovered plaintext.

### 4. Step-by-Step Visualization
The virtual lab displays:
- Input digraph
- Applied rule
- Output digraph
- Corresponding positions in the key square

Users can click on individual digraph rows to visualize the corresponding cells in the key square.

### 5. Interactive Quiz
The lab contains an interactive assessment covering:
- Playfair Cipher basics
- Key square construction
- I/J combination
- Digraph preparation
- Encryption rules
- Rectangle rule
- Security characteristics

### 6. Additional Features
- Dark mode
- Responsive layout
- Clear button
- Example messages
- Input validation
- Interactive navigation
- Visual highlighting of matrix cells

---

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Google Fonts

No external JavaScript libraries are required.

---

## Project Structure

```text
playfair-cipher/
│
├── index.html
└── README.md
