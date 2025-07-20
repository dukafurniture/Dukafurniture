<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Duka Furniture - Order Form</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: url('https://i.imgur.com/z0nTBSU.jpeg') no-repeat center center fixed;
      background-size: cover;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 600px;
      background: rgba(255, 255, 255, 0.95);
      margin: 50px auto;
      padding: 30px 40px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      position: relative;
    }

    .logo {
      text-align: center;
      margin-bottom: 20px;
    }

    .logo img {
      max-width: 180px;
      height: auto;
    }

    h1 {
      text-align: center;
      color: #b10000;
    }

    .slogan {
      text-align: center;
      font-style: italic;
      color: #333;
      margin-bottom: 20px;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input[type="text"],
    input[type="tel"],
    input[type="file"],
    select,
    textarea {
      width: 100%;
      padding: 10px;
      margin-top: 6px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 16px;
    }

    .signature {
      margin-top: 25px;
    }

    .signature label {
      font-weight: bold;
    }

    .signature input {
      border: none;
      border-bottom: 1px solid #000;
      width: 100%;
      background: transparent;
    }

    .legal {
      font-size: 13px;
      color: #555;
      margin-top: 20px;
      line-height: 1.4em;
    }

    .company-confirmation {
      margin-top: 30px;
      border-top: 1px dashed #888;
      padding-top: 20px;
    }

    .company-confirmation label {
      display: block;
      margin-top: 10px;
    }

    .company-confirmation input {
      border: none;
      border-bottom: 1px solid #000;
      width: 100%;
      background: transparent;
    }

    a.telegram-button,
    button[type="submit"] {
      display: block;
      text-align: center;
      background-color: #0088cc;
      color: #fff;
      padding: 14px;
      font-size: 18px;
      margin-top: 25px;
      border-radius: 6px;
      text-decoration: none;
      border: none;
      cursor: pointer;
    }

    a.telegram-button:hover,
    button[type="submit"]:hover {
      background-color: #0077b3;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="logo">
      <img src="https://i.imgur.com/GaB2IVT.png" alt="Duka Furniture Logo">
    </div>
    <h1>Duka Furniture - Custom Order</h1>
    <p class="slogan">የይርስዎ እቃ እና እስራልን፥</p>

    <form onsubmit="window.open('https://t.me/natway1','_blank'); return false;">
      <label for="name">Full Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="phone">Phone Number:</label>
      <input type="tel" id="phone" name="phone" required>

      <label for="furniture">Type of Furniture:</label>
      <select id="furniture" name="furniture">
        <option value="sofa">Sofa</option>
        <option value="table">Table</option>
        <option value="shelf">Shelf</option>
        <option value="bed">Bed</option>
        <option value="custom">Custom Design</option>
      </select>

      <label for="description">Details (Size, Color, Material, etc.):</label>
      <textarea id="description" name="description" rows="4"></textarea>

      <label for="design">Upload Design/Sketch (optional):</label>
      <input type="file" id="design" name="design" accept="image/*,application/pdf">

      <label for="address">Delivery Address:</label>
      <textarea id="address" name="address" rows="2" required></textarea>

      <div class="signature">
        <label for="signature">Signature (Type your full name as confirmation):</label>
        <input type="text" id="signature" name="signature" required>
      </div>

      <div class="company-confirmation">
        <strong>Company Confirmation (Duka Furniture):</strong>
        <label for="staffName">Staff Name (Receiving):</label>
        <input type="text" id="staffName" name="staffName">

        <label for="staffSignature">Staff Signature:</label>
        <input type="text" id="staffSignature" name="staffSignature">
      </div>

      <div class="legal">
        <strong>Legal Note:</strong><br>
        According to the <em>Ethiopian Civil Code Article 1675</em>, a contract is an agreement made by two or more persons to create, modify, or extinguish an obligation. Submitting this form confirms your acceptance of the offer, including furniture specifications, payment terms, and delivery.
      </div>

      <button type="submit">📤 Submit Order via Telegram</button>
    </form>
  </div>
</body>
</html>
