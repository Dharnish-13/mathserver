# Ex.05 Design a Website for Server Side Processing
# Date:
# AIM:
To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side.

# FORMULA:
P = I2R
P --> Power (in watts)
 I --> Intensity
 R --> Resistance

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Create python programs for views and urls to perform server side processing.

## Step 5:
Create a HTML file to implement form based input and output.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculate Power</title>
</head>
<body style="font-family: Arial, sans-serif; margin: 0; padding: 20px; background-color: #f4f4f4;">
    <div style="max-width: 600px; margin: auto; background: rgb(47, 237, 231); padding: 20px; border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
        <h1 style="text-align: center; color: #333;">Power Calculation (P = I²R)</h1>
        <form method="post" style="display: flex; flex-direction: column; gap: 15px;">
            {% csrf_token %}
            <label for="current" style="font-weight: bold; color: #555;">Current (I in Amperes):</label>
            <input type="number" step="any" name="current" id="current" required 
                   style="padding: 10px; border: 1px solid #ccc; border-radius: 5px; font-size: 16px;">

            <label for="resistance" style="font-weight: bold; color: #555;">Resistance (R in Ohms):</label>
            <input type="number" step="any" name="resistance" id="resistance" required 
                   style="padding: 10px; border: 1px solid #ccc; border-radius: 5px; font-size: 16px;">

            <button type="submit" 
                    style="padding: 10px 20px; border: none; border-radius: 5px; background-color: #000000; color: white; font-size: 16px; cursor: pointer;">
                Calculate
            </button>
        </form>

        {% if result is not None %}
        <div style="margin-top: 20px; padding: 10px; background-color: #f9f9f9; border: 1px solid #ddd; border-radius: 5px;">
            <h2 style="color: #333;">Result: {{ result }}</h2>
        </div>
        {% endif %}
    </div>
</body>
</html>
```
# SERVER SIDE PROCESSING:
<img width="1453" height="864" alt="Screenshot 2025-12-26 103258" src="https://github.com/user-attachments/assets/8d838028-fe4a-4055-a619-ec2916f6f354" />

# HOMEPAGE:
<img width="1443" height="791" alt="Screenshot 2025-12-26 103322" src="https://github.com/user-attachments/assets/2bef18db-94da-4636-8324-08ebf91fb6e1" />

# RESULT:
The program for performing server side processing is completed successfully.
