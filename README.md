# 🎨 Turtle Art - Rainbow Flower Pattern

This project creates a **rainbow-colored geometric flower spiral** using Python's `turtle` graphics and HSV color mapping.  
It generates a mesmerizing visual pattern with smooth color transitions. 🌈🐢

---

## 📸 Preview
*(You can add a screenshot of the output here once you run it. For example:)*  
![Preview of Turtle Art](preview.png)

---

## 🚀 Getting Started

### 1️⃣ Prerequisites
- Python 3.x installed  
- No external libraries required (only standard `turtle` and `colorsys`)

### 2️⃣ Installation
Clone the repository:
```bash
git clone https://github.com/yourusername/turtle-art.git
cd turtle-art
```
## 3️⃣ Run the Script
```bash
python main.py
```
## 📂 Project Structure
```bash
turtle-art/
│
├── rainbow_flower.py   # Main turtle art script
├── README.md           # Project documentation
└── preview.png         # (Optional) Screenshot of the output
```
## 🖌️ Code Overview
```python
from turtle import *
from colorsys import *

setposition(50, -50)
speed(0)
bgcolor('black')
pensize(2)

h = 0
for i in range(120):
    for j in range(4):
        color(hsv_to_rgb(h, 1, 1))
        h += 0.003
        circle(40+j*5, 90)
        forward(250)
        left(90)
    rt(10)

hideturtle()
done()
```
## 🌟 Features
✔ Generates colorful symmetric spiral patterns
✔ Uses HSV color model for smooth gradients
✔ Fast rendering with speed(0)
✔ Works on any OS with Python installed
## 💡 Customization
You can tweak:
- Number of iterations → range(120)
- Hue increment → h += 0.003
- Circle radius → circle(40+j*5, 90)
- Forward step → forward(250)
## 
