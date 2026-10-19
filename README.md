import random

# There are 20 icons in the app
icons = [f"icon{i}" for i in range(20)]

# Possible shapes
shapes = ["circle", "square", "triangle", "star", "heart"]


# Move every icon to a random position
def move_icons():
    for icon in icons:
        x = random.randint(0, 500)
        y = random.randint(0, 500)

        print(icon, "moved to", x, y)


# Give every icon a random color
def change_colors():
    for icon in icons:
        red = random.randint(0, 255)
        green = random.randint(0, 255)
        blue = random.randint(0, 255)

        color = f"rgb({red}, {green}, {blue})"

        print(icon, "changed to", color)


# Give every icon a random shape
def change_shapes():
    for icon in icons:
        shape = random.choice(shapes)

        print(icon, "changed to", shape)


# Simulate pressing the buttons
print("Move button:")
move_icons()

print("\nColor button:")
change_colors()

print("\nShape button:")
change_shapes()
