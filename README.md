<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>SwiftPesa Deposit</title>
</head>
<body>
  <h1>SwiftPesa Deposit App</h1>
  <button onclick="loginDeriv()">Login with Deriv</button>
  <br/><br/>
  <button onclick="depositMpesa()">Deposit via M-Pesa</button>
  <br/><br/>
  <a href="https://wa.me/254758419976" target="_blank">Contact Support on WhatsApp</a>

  <script>
    function loginDeriv() {
      const appId = '93522';
      const redirectUri = encodeURIComponent('https://madee391.github.io/deriv-oauth-redirect/');
      const markup = 2.5; // Your markup %
      const oauthUrl = `https://oauth.deriv.com/oauth2/authorize?app_id=${appId}&l=EN&redirect_uri=${redirectUri}&response_type=code&scope=read+payments&markup=${markup}`;
      window.location.href = oauthUrl;
    }

    function depositMpesa() {
      alert('M-Pesa deposit feature coming soon!');
      // You can later add payment integration here
    }
  </script>
</body>
</html>
