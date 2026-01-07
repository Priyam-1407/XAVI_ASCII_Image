

# Xavi Hernandez ASCII Art Generator

This project is a Python-based visualizer that reconstructs a portrait of legendary footballer **Xavi Hernandez** using a numerical grayscale matrix and ASCII character mapping.

1. What is an ASCII Image?
2. An ASCII Image is a form of digital art created using characters from the ASCII (American Standard Code for Information Interchange) table. Instead of using colored pixels, it relies on the visual density of different text characters to represent light and shadow.Darker Tones: Represented by "dense" or "heavy" characters like @, #, and %.Lighter Tones/Outlines: Represented by "light" or "thin" characters like ., :, -, and +.Significance: This allows images to be rendered on systems that do not support traditional graphics, such as older hardware, command-line interfaces, and simple text editors.

   Project Overview
4. The XAVI Renderer is a Python-based application that reconstructs a complex visual image (4:5 aspect ratio) directly within the terminal window. This project serves as a practical demonstration of how coordinate-based data can be translated into a visual display using fundamental programming concepts.

5. Technical Objectives:

 Hardcoded Reconstruction:
 To recreate a specific visual without external image dependencies.Algorithmic Rendering: To manage a grid of 1,080 character points ($27$ rows by $40$ columns).
User Experience: To implement a sequential rendering effect using time delays.3. Technical Implementation: Loops and Conditional LogicThe project is built on the foundation of Nested Iteration and Complex Conditional Branching.A. The Role of Nested LoopsThe script utilizes a two-tier loop system to navigate the terminal "canvas":
Outer Loop (for row in range(height)): This loop controls the vertical movement, moving the cursor from the top of the terminal to the bottom for 27 iterations.
Inner Loop (for col in range(width)): For every single row, this inner loop moves horizontally across 40 columns to determine the character for each specific coordinate.


B. The Decision Engine (If-Else & Elif)To decide which character belongs at a specific coordinate (row, col), the project uses a massive engine of conditional statements.Point-Specific Mapping: Some characters are assigned to a single coordinate (e.g., if col == 0: char = "-") to define sharp edges or specific details.Range-Based Mapping: To create solid shapes or textures efficiently, the script uses comparison operators to fill a range of columns (e.g., elif 23 <= col <= 25: char = "@").Layering with Elif: The use of elif ensures that the script checks conditions in a specific priority, allowing the image to have "layers" of depth and complex shading.4. Animation and RenderingTo prevent the image from appearing instantly, the time module is utilized:Line Delay: A time.sleep(0.05) delay is added at the end of each row iteration.Visual Effect: This creates a scanning effect similar to how old CRT monitors or 3D printers build a scene layer by layer.


By:
PRIYAM TIWARI
AIML
RUNGTA COLLEGE OF ENGINEERING AND TECHNOLOGY


