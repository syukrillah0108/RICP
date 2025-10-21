# SIKLUS PENGOLAHAN SAMPAH

![](./img/siklus-sampah.svg)

# PROSES PENGOLAHAN SAMPAH

## 1. Eco-Enzyme

### Takaran

| No | Bahan      | Jumlah |
| -- | ---------- | ------ |
| 1  | Air        | 60%    |
| 2  | Bahan Baku | 30%    |
| 3  | Gula Merah | 10%    |

### Kalkulator Eco-Enzyme
<div>
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kalkulator Eco-Enzyme</title>
<style>
  body {
    background: #f8f9fa;
    font-family: Arial, sans-serif;
  }
  #eco-enzyme-calculator {
    max-width: 400px;
    margin: 50px auto;
    background: white;
    padding: 15px;
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  }
  h3 { text-align: center; color: #2c3e50; }
  input, button {
    width: 100%;
    padding: 8px;
    margin-top: 8px;
    border-radius: 8px;
    border: 1px solid #ccc;
  }
  button {
    background: #27ae60;
    color: white;
    border: none;
    cursor: pointer;
  }
  button:hover {
    background: #219150;
  }
</style>
</head>
<body>
<div id="eco-enzyme-calculator">
  <h3>Kalkulator Eco-Enzyme</h3>
  <p>Masukkan total campuran (gram):</p>
  <input id="totalWeight" type="number" placeholder="Masukkan total gram">
  <button id="calculate">Hitung</button>
  <div id="result">
    <p>Air: -</p>
    <p>Bahan Baku: -</p>
    <p>Gula Merah: -</p>
  </div>
</div>

<script>
document.getElementById('calculate').addEventListener('click', function() {
  const total = parseFloat(document.getElementById('totalWeight').value);
  if (isNaN(total) || total <= 0) {
    alert('Masukkan total gram yang valid!');
    return;
  }
  const air = total * 0.6;
  const bahanBaku = total * 0.3;
  const gulaMerah = total * 0.1;

  document.getElementById('result').innerHTML = `
    <p>💧 Air: <b>${air.toFixed(2)} g</b></p>
    <p>🍂 Bahan Baku: <b>${bahanBaku.toFixed(2)} g</b></p>
    <p>🍯 Gula Merah: <b>${gulaMerah.toFixed(2)} g</b></p>
  `;
});
</script>
</body>
</html>

</div>

