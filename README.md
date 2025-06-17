##🧺 Fuzzy Logic Washing Machine Controller

This project implements a fuzzy logic system to simulate decision-making in a smart washing machine. Using fuzzy logic, the system determines the optimal wash time, water temperature, and spin speed based on input parameters like load size, fabric type, and dirt level.

###🔍 Overview
Traditional washing machines operate using predefined cycles. In contrast, this fuzzy logic-based controller adjusts its output dynamically based on the characteristics of the laundry load, offering a more intelligent and efficient approach.

📊 Input Variables
Load Size (0–8 kg)

Fabric Type (1–5 scale, from Very Delicate to Very Tough)

Dirt Level (0–100%)

🎯 Output Variables
1. Wash Time (5–60 minutes)
2. Water Temperature (20–90 °C)
3. Spin Speed (0–1200 rpm)

🧠 Fuzzy Logic Rules
A set of fuzzy rules is defined to control the output based on combinations of inputs. For example:

```
IF Load Size is Very Light AND Fabric Type is Very Delicate AND Dirt Level is Light
THEN Wash Time is Very Short, Water Temperature is Cold, Spin Speed is Very Gentle
```

⚙️ How It Works
1. Define fuzzy membership functions for all input and output variables.

2. Set up rules that connect the inputs to outputs.

3. Use skfuzzy to simulate the control system based on a given scenario.

🚀 Getting Started
Requirements

-Python 3.x

-NumPy

-scikit-fuzzy (pip install scikit-fuzzy)

Run the Simulation:
```
python fuzzy_washing_machine.py
```

*Sample Output*

Available Outputs: {'Wash Time': 23.45, 'Water Temperature': 38.72, 'Spin Speed': 520.39}
Wash Time: 23.45 minutes
Water Temperature: 38.72 °C
Spin Speed: 520.39 rpm

📈 Visualization
The script includes graphical visualization of the membership functions using matplotlib.

📁 File Structure

├── fuzzy_washing_machine.py   # Main simulation script

├── README.md                  # Project description

🧠 Concepts Used

-Fuzzy Membership Functions: trapezoidal & triangular

-Fuzzy Rules & Inference

-Control system simulation using skfuzzy

📌 Future Enhancements

-Add more rules to cover a broader range of input combinations

-Build a GUI to let users select inputs interactively

-Integrate real sensor input for real-time decision making


🤝 Contributing

Feel free to fork the repo and open a pull request to improve rules, add more fuzzy sets, or optimize the inference system.
