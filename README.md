# 📌 Stock Price Alert via SMS using Twilio
<h2>✅ Project Description:</h2>
<p>This project tracks the daily stock price of a specified company (in this case, Tesla Inc. - stock symbol TSLA) using the Alpha Vantage API. It compares the closing stock prices of the last two days to check if there is a significant percentage change (greater than 5% by default).</p>
<h3>🧱 Modules Used:</h3>
<p><strong>🔹 Standard Libraries:</strong></p>
<ul>
  <li><strong>requests:</strong> For making HTTP requests to the APIs.</li>
  <li><strong>json (implicitly used):</strong> To parse the JSON responses.</li>
</ul>
<p><strong>🔹 Third-party Libraries:</strong></p>
<ul>
  <li><strong>twilio.rest.Client:</strong> Twilio's official Python SDK for sending SMS.</li>
</ul>
<h3>APIs and Services Used:</h3>
<ol>
  <li>1. 📈 Alpha Vantage API
    <ul>
      <li><strong>Purpose:</strong> To get daily stock price data.</li>
      <li><strong>Endpoint:<strong></strong>
        <p>https://www.alphavantage.co/query</p>
      <li><strong>API Key Required:</strong> ✅ Yes (e.g., CO9RGDLPS1QXVK0G)</li>
      <li><strong>Documentation:</strong> <a href="https://newsapi.org/docs/endpoints/everything" target="_blank">View Docs</a></li>
    </ul>
  </li>
  <li>2. 📰 News API
    <ul>
      <li><strong>Purpose:</strong> To fetch recent news articles related to a company.</li>
      <li><strong>Endpoint:</strong>
        <p>https://newsapi.org/v2/everything</p></li>
      <li><strong>API Key Required:</strong> ✅ Yes (e.g., 18901e9cb31d4764922ab164a985c750)</li>
      <li><strong>Documentation:</strong> <a href="https://newsapi.org/docs/endpoints/everything" target="_blank">View Docs</a></li>
    </ul>
  </li>
  <li>3. 📱 Twilio SMS API
    <ul>
      <li><strong>Purpose:</strong> To send SMS alerts containing stock info and news headlines.</li>
      <li><strong>Signup:</strong> <a href="https://www.twilio.com/try-twilio" target="_blank">Create Free Account</a></li>
      <li><strong>SMS Documentation:</strong> <a href="https://www.twilio.com/docs/sms/send-messages" target="_blank">View Docs</a></li>
    </ul>
  </li>
</ol>
