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
  <li> 📈 Alpha Vantage API
    <ul>
      <li><strong>Purpose:</strong> To get daily stock price data.</li>
      <li><strong>Endpoint:<strong></strong>
        <p>https://www.alphavantage.co/query</p>
      <li><strong>API Key Required:</strong> ✅ Yes (e.g., CO9RGDLPS1QXVK0G)</li>
      <li><strong>Documentation:</strong> <a href="https://newsapi.org/docs/endpoints/everything" target="_blank">View Docs</a></li>
    </ul>
  </li>
  <li> 📰 News API
    <ul>
      <li><strong>Purpose:</strong> To fetch recent news articles related to a company.</li>
      <li><strong>Endpoint:</strong>
        <p>https://newsapi.org/v2/everything</p></li>
      <li><strong>API Key Required:</strong> ✅ Yes (e.g., 18901e9cb31d4764922ab164a985c750)</li>
      <li><strong>Documentation:</strong> <a href="https://newsapi.org/docs/endpoints/everything" target="_blank">View Docs</a></li>
    </ul>
  </li>
  <li> 📱 Twilio SMS API
    <ul>
      <li><strong>Purpose:</strong> To send SMS alerts containing stock info and news headlines.</li>
      <li><strong>Signup:</strong> <a href="https://www.twilio.com/try-twilio" target="_blank">Create Free Account</a></li>
      <li><strong>SMS Documentation:</strong> <a href="https://www.twilio.com/docs/sms/send-messages" target="_blank">View Docs</a></li>
    </ul>
  </li>
</ol><br>
<h3>Twilio Setup Guide (for SMS Sending)</h3>
<p><strong>Step 1: Create a Twilio Account</strong></p>
<ol>
  <li>Go to <a href="https://www.twilio.com/" target="_blank">https://www.twilio.com/</a></li>
  <li>Click on Sign Up (if you don't have an account) or Log In</li>
  <li>Verify your email and phone number.</li>
</ol>
<p><strong>📱 Step 2: Get a Twilio Phone Number</strong></strong></p>
<ol>
  <li>Go to your <a href="https://console.twilio.com/" target="_blank">Twilio Console Dashboard</a></li>
  <li>Click on Get a Twilio Phone Number</li>
  <li>Choose a number with SMS capability</li>
  <li>Note down the phone number — you'll use this as the from_ number in your code.</li>
</ol>
<p><strong>🔐 Step 3: Get Twilio Account SID and Auth Token</strong></p>
<ol>
  <li>From the Dashboard, copy the following:
    <ul>
      <li><strong>Account SID →</strong> used for authentication</li>
      <li><strong>Auth Token →</strong> keep this private</li>
    </ul>
  </li>
  <li>You’ll use these in your code:</li><br>
  <p>account_sid = "YOUR_TWILIO_ACCOUNT_SID"<br>
    auth_token = "YOUR_TWILIO_AUTH_TOKEN"</p>
</ol>
<h3>💬 Step 4: Verify Recipient Phone Number (for Trial Account)</h3>
<p>If you're using a <strong>free trial account</strong>, Twilio <strong>only allows SMS to verified phone numbers:</strong></p>
<ol>
   <li>Go to: <a href="https://console.twilio.com/us1/verified-caller-ids/phone-numbers" target="_blank">Verified Caller IDs</a>
   <li>Click <strong>Add a New Verified Number</strong></li>
   <li>Enter your personal phone number and verify it via OTP.</li>
</ol><br>
