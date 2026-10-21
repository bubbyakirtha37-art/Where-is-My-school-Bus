
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Where Is My School Bus?</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f1f5f9;
      color: #17345c;
    }
    header {
      background: #123b72;
      color: white;
      padding: 30px 16px;
      text-align: center;
    }
    header h1 { font-size: 27px; margin: 0 0 10px; }
    main { max-width: 600px; margin: 24px auto; padding: 16px; }
    .card {
      background: white;
      border-radius: 16px;
      padding: 22px;
      margin-bottom: 18px;
      box-shadow: 0 4px 14px #0000000d;
    }
    button {
      width: 100%;
      padding: 14px;
      margin-top: 10px;
      border: 0;
      border-radius: 9px;
      background: #1769e0;
      color: white;
      font-size: 16px;
    }
    .status { color: #a15c00; font-weight: bold; }
    #message { line-height: 1.5; }
    footer { text-align: center; padding: 20px; color: #64748b; }
  </style>
</head>
<body>
  <header>
    <h1>🚌 Where Is My School Bus?</h1>
    <p>Every journey, right on time.</p>
  </header>

  <main>
    <section class="card">
      <h2>Welcome!</h2>
      <p>Know where your school bus is, wherever you are.</p>
      <p class="status">Demo version — live tracking is not connected yet.</p>
    </section>

    <section class="card">
      <h2>My School Bus</h2>
      <p>Bus number: Not assigned</p>
      <p>Bus status: Waiting for connection</p>
      <button onclick="showMessage('Live bus tracking will be available after GPS and Firebase setup.')">
        Track My Bus
      </button>
      <button onclick="showMessage('Your assigned bus stop will appear after your school account is connected.')">
        My Stop
      </button>
      <button onclick="showMessage('Your bus route will appear after your school sets it up.')">
        View Route
      </button>
      <p id="message" aria-live="polite"></p>
    </section>
  </main>

  <footer>Where Is My School Bus? © 2026</footer>

  <script>
    function showMessage(text) {
      document.getElementById("message").textContent = text;
    }
  </script>
</body>
</html>
# Where-is-My-school-Bus
School bus tracking app
