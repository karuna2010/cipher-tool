# cipher-tool<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Cipher Tool - Caesar Cipher</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    h1 {
      color: #333;
    }

    .cipher-container {
      max-width: 500px;
      width: 100%;
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    textarea, input[type="number"], select, button {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      margin-bottom: 20px;
      font-size: 16px;
    }

    button {
      background-color: #007bff;
      color: white;
      border: none;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }

    .output {
      background-color: #f1f1f1;
      padding: 10px;
      min-height: 50px;
      white-space: pre-wrap;
      word-wrap: break-word;
    }

    footer {
      margin-top: 40px;
      font-size: 14px;
      color: #888;
    }
  </style>
</head>
<body>

  <h1>🔐 Caesar Cipher Tool</h1>
  <div class="cipher-container">
    <label for="message">Enter your message:</label>
    <textarea id="message" rows="4" placeholder="Type here..."></textarea>

    <label for="shift">Shift (Key):</label>
    <input type="number" id="shift" value="3" />

    <label for="action">Action:</label>
    <select id="action">
      <option value="encrypt">Encrypt</option>
      <option value="decrypt">Decrypt</option>
    </select>

    <button onclick="processCipher()">Run Cipher</button>

    <h3>Output:</h3>
    <div clas
