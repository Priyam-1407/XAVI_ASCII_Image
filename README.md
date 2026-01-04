

# Xavi Hernandez ASCII Art Generator

This project is a Python-based visualizer that reconstructs a portrait of legendary footballer **Xavi Hernandez** using a numerical grayscale matrix and ASCII character mapping.

## 📝 Project Overview

The goal of this project is to demonstrate how digital images are represented as data and how that data can be translated into a text-based visual format. By treating a terminal window as a canvas and characters as pixels, we recreate a recognizable image using nothing but standard Python logic.

## 🎨 What is ASCII Art?

**ASCII Art** is a graphic design technique that uses printable characters from the ASCII standard (letters, numbers, and symbols) to create a visual image.

* It dates back to early computing when graphical displays were limited.
* Instead of pixels, it uses the **visual density** of characters—for example, `@` looks darker because it fills more space, while `.` looks lighter because it leaves more empty space.

## 🛠️ How We Built This

The project follows a three-step data transformation process:

### 1. Numerical Representation (The Matrix)

The image is stored as a 2D list (matrix) named `face`. Each number in this matrix represents the **grayscale intensity** of a specific "pixel":

* **High values (e.g., 247)** represent darker areas like hair or deep shadows.
* **Low values (e.g., 21)** represent highlights or bright background areas.

### 2. Character Mapping (The Dictionary)

We created a mapping dictionary `gray_to_char` that links each numerical intensity to a specific ASCII character based on its weight:

* **Darkest:** `247 -> @`
* **Mid-tones:** `129 -> +`
* **Lightest:** `21 -> .`

### 3. The Reconstruction Loop

The Python script iterates through the 2D matrix. For every numerical value it finds, it lookups the corresponding character in our dictionary and prints it to the terminal.

```python
for row in face:
    for val in row:
        # Translates number to character and prints without a newline
        print(gray_to_char[val], end='')
    print() # Moves to the next line after finishing a row

```

## 🎯 Key Learning Objectives

* **Data Mapping:** Understanding how to translate one set of data (numbers) into another (symbols).
* **Matrix Traversal:** Learning how to process 2D arrays efficiently using nested loops.
* **Image Processing Fundamentals:** Gaining insight into how computers perceive images as grids of intensity values.

By:
PRIYAM TIWARI
AIML
RUNGTA COLLEGE OF ENGINEERING AND TECHNOLOGY


