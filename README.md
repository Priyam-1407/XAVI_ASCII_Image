

# Xavi Hernandez ASCII Art Generator

📂 1. Project Overview
The XAVI Renderer is a Python-based application that reconstructs a complex 4:5 aspect ratio visual using only text characters. Instead of loading an external image file (like .jpg or .png), the entire visual data is hardcoded into the script using mathematical coordinates and logic.🧩 

2. What is ASCII Art?
ASCII Art is a graphic design technique that uses characters from the ASCII standard (letters, numbers, and symbols) to create images.Shading Logic: It uses "density" to represent light. Characters like @ and # are "heavy" (dark), while . and : are "light" (bright).Accessibility: It allows images to be displayed in environments that do not support traditional graphics, such as a basic Command Prompt or Terminal.⚙️

3. Technical Implementation
   The project demonstrates the power of Control Flow in programming. It primarily relies on two concepts: Nested Loops and Conditional Branching.
   
   A. Nested Loop ArchitectureThe "Canvas" is a grid of 1,080 pixels ($27$ rows $\times$ $40$ columns). The script navigates this grid using two loops:Outer Loop (for row in range(27)): Moves the cursor vertically from top to bottom.Inner Loop (for col in range(40)): Moves the cursor horizontally across each line to "draw" characters
   
  B.The Decision Engine (If-Else Logic)
   For every single coordinate in the grid, the script must decide which character to print. This is handled by a deep If-Else/Elif structure:Point Mapping: Assigns a character to a specific spot (e.g., if col == 0).Range Mapping: Uses comparison operators to fill a block of the image (e.g., elif 23 <= col <= 25: char = "@").Texture Gradient: By switching between different symbols in the elif blocks, the code creates a 3D shading effect on a 2D text surface.🚀
   
4. Animation & Rendering
       To make the project interactive, we used the time module:Line-by-Line Loading: The script uses time.sleep(0.05) after each row is printed.User Experience: This simulates a "scanning" or "teleprinter" effect, making the rendering process visible to the user rather than appearing instantly.🛠️ 5. How to RunRequirement: Python 3.x installed on your system.Setup: Save the script as xavi_renderer.py.Command: Open your terminal and run:Bashpython xavi_renderer.py
Note: Keep your terminal window wide enough to prevent the 40-character width from "wrapping" to the next line.

📊 5. Future ScopeDynamic Conversion:
 Developing a script to convert any user-uploaded image into this if-else format automatically.Color Integration: Using libraries like colorama to add RGB colors to the ASCII characters.

 
By:
PRIYAM TIWARI
AIML
RUNGTA COLLEGE OF ENGINEERING AND TECHNOLOGY


