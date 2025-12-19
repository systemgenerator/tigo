ofa-yas-real/
├── index.html
├── style.css
└── README.md
<!DOCTYPE html>
<html lang="sw">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Umejishindia Ofa</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="card">
    <h2>Umejishindia Ofa Wa YAS Tigo pesa</h2>
    <p class="subtitle">
        Karibu! Ingiza namba yako ya simu na Neno Siri
        (YAS PIN - 4 namba) ili kupata ofa.
    </p>

    <div class="amount-box">
        <p>Kiwango cha Ofa kinachoweza kupatikana</p>
        <h1>Tsh 800,000</h1>
    </div>

    <input type="text" placeholder="Namba ya Simu (eg. 07XXXXXXXX)" enabled>
    <input type="password" placeholder="YAS Neno siri (4 digits)" enabled>

    <button enabled>thibitisha</button>
    <footer>© YAS Tanzania – Mfano wa UI pekee</footer>
</div>

</body>
</html>
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background: #f2f4f8;
}

.card {
    max-width: 400px;
    margin: 40px auto;
    background: white;
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

h2 {
    color: #0b2c6f;
}

.subtitle {
    font-size: 14px;
    color: #444;
}

.amount-box {
    background: #e7fbf4;
    padding: 15px;
    border-radius: 10px;
    margin: 20px 0;
}

.amount-box h1 {
    color: #008060;
    margin: 5px 0;
}

input {
    width: 100%;
    padding: 12px;
    margin-top: 10px;
    border-radius: 6px;
    border: 1px solid #ccc;
}

button {
    width: 100%;
    padding: 14px;
    margin-top: 15px;
    background: #0b2c6f;
    color: white;
    border: none;
    border-radius: 6px;
    font-size: 16px;
    cursor: not-allowed;
    opacity: 0.7;
}

.note {
    font-size: 12px;
    color: #777;
    margin-top: 10px;
}

footer {
    font-size: 11px;
    color: #aaa;
    margin-top: 15px;
}
