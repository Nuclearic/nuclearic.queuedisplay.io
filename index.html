<!DOCTYPE html>
<html>
<head>
  <title>Order Display</title>
  <meta name="viewport" content="width=640, initial-scale=1.0">
  <style>
    html, body {
      width: 100%;
      height: 100%;
      margin: 0;
      padding: 0;
      font-family: sans-serif;
      background: white;
      color: black;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
    }

    h1 {
      font-size: 2em;
      margin: 20px;
    }

    #displayOrders {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-gap: 10px;
      width: 90%;
      padding: 10px;
      box-sizing: border-box;
    }

    .order {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 150px;
      border: 2px solid black;
      border-radius: 10px;
      font-size: 2em;
      background: #f0f0f0;
    }

    #hiddenInput {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      opacity: 0;
      z-index: 1;
    }
  </style>
</head>
<body>
  <h1>Now Serving</h1>
  <div id="displayOrders"></div>

  <audio id="ding" src="https://www.orangefreesounds.com/wp-content/uploads/2021/01/Ding-dong-sound.mp3" preload="auto"></audio>

  <input type="text" id="hiddenInput" onkeydown="handleKey(event)" autocomplete="off" autofocus />

  <script>
    let orders = [];

    function showOrders() {
      const display = document.getElementById('displayOrders');
      display.innerHTML = '';
      orders.forEach(order => {
        const div = document.createElement('div');
        div.className = 'order';
        div.textContent = order;
        display.appendChild(div);
      });
    }

    function playDing() {
      const ding = document.getElementById('ding');
      ding.pause();
      ding.currentTime = 0;
      ding.play().catch(err => console.log("Sound error:", err));
    }

    function addOrder(order) {
      orders.unshift(order);
      if (orders.length > 10) orders = orders.slice(0, 10);
      localStorage.setItem('orders', JSON.stringify(orders));
      showOrders();
      playDing();
    }

    function handleKey(e) {
      if (e.key === 'Enter') {
        const value = e.target.value.trim();
        if (value) {
          addOrder(value);
        }
        e.target.value = '';
      }
    }

    window.onload = () => {
      const saved = localStorage.getItem('orders');
      if (saved) orders = JSON.parse(saved);
      showOrders();

      const input = document.getElementById('hiddenInput');
      input.focus();

      window.addEventListener('click', () => input.focus());
      window.addEventListener('keydown', () => input.focus());
    };

    window.addEventListener('storage', function (e) {
      if (e.key === 'orders') {
        orders = JSON.parse(e.newValue || '[]');
        showOrders();
        playDing();
      }
    });
  </script>
</body>
</html>
