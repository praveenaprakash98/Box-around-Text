# Box-around-Text
How does the Python script in the image create a box around the entered text?


The code dynamically creates a text box based on the user’s input. It calculates spacing to center the text within the box and then prints formatted borders using plus (+), dash (-), and pipe (|) characters. The output section showcases the effect, displaying "Data Science" inside a neatly formatted box.

1️⃣ Accept User Input
The program first asks the user to enter a string (e.g., "Data Science").
text = input("Enter your text: ")


2️⃣ Calculate Box Size
- The width of the box is determined by the length of the text.
- It adds some padding (usually spaces or symbols) to ensure proper alignment.


3️⃣ Generate Box Borders
The top and bottom borders are made of + and - characters:
border = "+" + "-" * len(text) + "+"


- "-" * len(text) ensures the box fits the text exactly.
- + is added at both ends for the border corners.

The middle section contains the text:
content = "|" + text + "|"


- The | symbols create side borders.


4️⃣ Print the Box
Finally, the script prints the formatted output in three steps:
print(border)   # Top border
print(content)  # Text inside box
print(border)   # Bottom border


Example Output
If the user enters "Data Science", the program generates:
+-------------+
|Data Science|
+-------------+
