# Ex.04 Design a Website for Server Side Processing
## Date:

## AIM:
To create a web page to calculate total bill amount with GST from price and GST percentage, using server-side scripts.

## FORMULA:
Bill = P + (P * GST / 100)
<br> P --> Price (in Rupees)
<br> GST --> GST (in Percentage)
<br> Bill --> Total Bill Amount (in Rupees)

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Power Calculator</title>
  <style>
    body {
      background-color: #f5f3ce;
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover;
      text-align: center;
      font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
      color: brown;
      margin: 0;
      padding: 0;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 20px;
    }

    .container {
      background-color: #c9c4b7;
      padding: 75px 40px;
      clip-path: polygon(
        25% 6.7%, 75% 6.7%, 
        100% 50%, 75% 93.3%, 
        25% 93.3%, 0% 50%
      );
      width: 400px;
      margin: 100px auto;
      box-shadow: 0 0 15px #1fe374;
    }

    label {
      font-size: 1.5em;
      display: block;
      margin: 15px 0 5px;
    }

    input[type="text"] {
      width: 75%;
      padding: 10px;
      border-radius: 12px;
      border: 1px solid #051313;
      margin-bottom: 15px;
      font-size: 1em;
    }

    input[type="submit"] {
      background-color: #1fe374;
      color: rgb(211, 241, 247);
      border: none;
      border-radius: 10px;
      padding: 10px 21px;
      font-size: 1em;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    input[type="submit"]:hover {
      background-color: #d588b2;
    }

    p {
      font-size: 1.2em;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>The Power of the Bulb</h1>
    <form method="POST">
      {% csrf_token %}
      <label>Intensity (A):</label>
      <input type="text" name="intensity" value="{{I}}" />

      <label>Resistance (Ohm):</label>
      <input type="text" name="resistance" value="{{R}}" />

      <input type="submit" value="Calculate" />

      <label>Power (Watts):</label>
      <input type="text" name="power" value="{{power}}" />
    </form>
  </div>
</body>
</html>
```

## OUTPUT - SERVER SIDE:

<img width="1780" height="1076" alt="image" src="https://github.com/user-attachments/assets/48adfc26-dd39-424a-b880-cae080a18d1d" />

## OUTPUT - WEBPAGE:

<img width="1205" height="1031" alt="image" src="https://github.com/user-attachments/assets/acb737f7-3215-4eaa-beb9-9c6ad1921fd0" />

## RESULT:
The a web page to calculate vehicle mileage and fuel efficiency using server-side scripts is created successfully.
