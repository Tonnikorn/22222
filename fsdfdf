<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ซื้อขายเห็ดแดง</title>
<style>
    body {
        font-family: 'Arial', sans-serif;
        background-color: #FFF5E6;
        margin: 0;
        padding: 0;
    }
    .container {
        max-width: 400px;
        margin: 20px auto;
        background-color: #FFFAF0;
        padding: 30px;
        border-radius: 20px;
        box-shadow: 0 0 15px rgba(0,0,0,0.2);
    }
    h1 { 
        text-align: center; 
        color: #C1272D; 
        margin-bottom: 30px; 
        font-size: 32px; 
    }
    label { 
        display: block; 
        font-size: 22px; 
        margin-top: 15px; 
    }
    input[type="number"] {
        width: 100%; 
        padding: 12px; 
        font-size: 22px;
        border-radius: 10px; 
        border: 1px solid #CCC; 
        margin-top: 5px;
    }
    button {
        width: 100%; 
        padding: 15px; 
        font-size: 24px;
        background-color: #C1272D; 
        color: white; 
        border: none;
        border-radius: 15px; 
        cursor: pointer; 
        margin-top: 25px;
    }
    button:hover { background-color: #FF4C4C; }
    .result { 
        margin-top: 25px; 
        font-size: 26px; 
        font-weight: bold; 
        text-align: center; 
        color: #1C6E8C; 
        line-height: 1.8;
    }
    @media (max-width: 500px) {
        h1 { font-size: 28px; } 
        label { font-size: 20px; } 
        input[type="number"] { font-size: 20px; } 
        button { font-size: 22px; } 
        .result { font-size: 24px; }
    }
</style>
</head>
<body>
<div class="container">
    <h1>ซื้อขายเห็ดแดง</h1>

    <label for="small">จี๋เล็ก (กิโลกรัม):</label>
    <input type="number" id="small" min="0" placeholder="กรอกตัวเลขเท่านั้น" inputmode="decimal">

    <label for="large">จี๋ใหญ่ (กิโลกรัม):</label>
    <input type="number" id="large" min="0" placeholder="กรอกตัวเลขเท่านั้น" inputmode="decimal">

    <label for="bloom">เห็ดบาน (กิโลกรัม):</label>
    <input type="number" id="bloom" min="0" placeholder="กรอกตัวเลขเท่านั้น" inputmode="decimal">

    <button type="button" id="calculateBtn">คำนวณราคา</button>

    <div class="result" id="total"></div>
</div>

<script>
document.getElementById('calculateBtn').addEventListener('click', function() {
    const priceSmall = 100;
    const priceLarge = 290;
    const priceBloom = 70;

    const small = parseFloat(document.getElementById('small').value) || 0;
    const large = parseFloat(document.getElementById('large').value) || 0;
    const bloom = parseFloat(document.getElementById('bloom').value) || 0;

    const totalSmall = small * priceSmall;
    const totalLarge = large * priceLarge;
    const totalBloom = bloom * priceBloom;
    const total = totalSmall + totalLarge + totalBloom;

    document.getElementById('total').innerHTML = `
        จี๋เล็ก: ${totalSmall.toLocaleString()} บาท<br>
        จี๋ใหญ่: ${totalLarge.toLocaleString()} บาท<br>
        เห็ดบาน: ${totalBloom.toLocaleString()} บาท<br>
        <strong>จำนวนเงินทั้งหมด: ${total.toLocaleString()} บาท</strong>
    `;
});
</script>
</body>
</html>
