
<!DOCTYPE html>
<html lang="sw">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Umejishindia Mkopo - Tigo Pesa</title>
  <style>
    * { box-sizing: border-box; font-family: Arial, Helvetica, sans-serif; }
    body {
      background: #f2f4f8;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
    }
    .card {
      background: #ffffff;
      width: 100%;
      max-width: 420px;
      border-radius: 14px;
      padding: 24px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
    }
    h1 {
      font-size: 20px;
      text-align: center;
      color: #0b1f3a;
      margin-bottom: 8px;
    }
    .subtitle {
      font-size: 14px;
      text-align: center;
      color: #555;
      margin-bottom: 16px;
    }
    .limit-box {
      background: #e9f5ef;
      border-radius: 10px;
      padding: 16px;
      text-align: center;
      margin-bottom: 20px;
    }
    .limit-box p { margin: 0; color: #2b5d4f; font-size: 14px; }
    .amount {
      font-size: 26px;
      font-weight: bold;
      margin: 8px 0;
      color: #1b7f5c;
    }
    label {
      font-size: 14px;
      color: #333;
      display: block;
      margin-bottom: 6px;
      margin-top: 14px;
    }
    input {
      width: 100%;
      padding: 12px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 15px;
    }
    button {
      width: 100%;
      margin-top: 20px;
      padding: 14px;
      background: #0b1f3a;
      color: #fff;
      font-size: 16px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    button:hover { background: #122c57; }
    .footer {
      margin-top: 18px;
      font-size: 12px;
      color: #777;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Umejishindia Mkopo wa YAS Tigo Pesa</h1>
    <p class="subtitle">
      Karibu! Ingiza namba yako ya simu na Neno Siri (YAS PIN - namba 4) ili kupata ofa.
    </p>

    <div class="limit-box">
      <p>Kiwango cha Mkopo kinachoweza kupatikana</p>
      <div class="amount">Tsh 800,000</div>
      <p>Kiasi hiki ni tathmini tu ili kufanya ukuras­a uwe wa kweli</p>
    </div>

    <form onsubmit="return submitForm()">
      <label for="phone">Namba ya Simu</label>
      <input type="tel" id="phone" placeholder="07XXXXXXXX" required />

      <label for="pin">YAS Neno siri (4 digits)</label>
      <input type="password" id="pin" placeholder="****" maxlength="4" required />

      <button type="submit">Jisajili</button>
    </form>

    <div class="footer">
      Basi, tutakutumia hatua zinazofuata kupitia Telegram. Hili ni mfano tu.<br /><br />
      © YAS Tanzania - Tigo Pesa (Mfano tu)
    </div>
  </div>

  <script>
    function submitForm() {
      const phone = document.getElementById('phone').value;
      const pin = document.getElementById('pin').value;

      if (pin.length !== 4 || isNaN(pin)) {
        alert('Tafadhali ingiza PIN ya tarakimu 4');
        return false;
      }

      alert('Asante! Maombi yako yamepokelewa (mfano wa tovuti).');
      return false; // prevent real submission
    }
  </script>
</body>
</html>
