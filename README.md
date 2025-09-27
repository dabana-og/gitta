<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Simple HTML Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 40px;
      background-color: #f4f4f4;
    }

    h2 {
      color: #333;
    }

    form {
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      width: 400px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    label {
      display: block;
      margin-top: 10px;
      font-weight: bold;
    }

    input[type="text"],
    input[type="email"],
    input[type="password"],
    select,
    textarea {
      width: 100%;
      padding: 8px;
      margin-top: 4px;
      box-sizing: border-box;
    }

    input[type="submit"] {
      margin-top: 20px;
      background-color: #4285F4;
      color: white;
      border: none;
      padding: 10px 15px;
      cursor: pointer;
      border-radius: 4px;
    }

    input[type="submit"]:hover {
      background-color: #3367D6;
    }
  </style>
</head>
<body>

  <h2>Registration Form</h2>

  <form action="/submit-form" method="POST">
    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required>

    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>

    <label>Gender:</label>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male" style="font-weight: normal;">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female" style="font-weight: normal;">Female</label>

    <label>Hobbies:</label>
    <input type="checkbox" id="reading" name="hobbies" value="reading">
    <label for="reading" style="font-weight: normal;">Reading</label>
    <input type="checkbox" id="traveling" name="hobbies" value="traveling">
    <label for="traveling" style="font-weight: normal;">Traveling</label>
    <input type="checkbox" id="gaming" name="hobbies" value="gaming">
    <label for="gaming" style="font-weight: normal;">Gaming</label>

    <label for="country">Country:</label>
    <select id="country" name="country">
      <option value="usa">United States</option>
      <option value="uk">United Kingdom</option>
      <option value="canada">Canada</option>
      <option value="australia">Australia</option>
    </select>

    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4"></textarea>

    <input type="submit" value="Submit">
  </form>

</body>
</html>
