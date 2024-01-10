<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>best earning
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Earnings Wallet</h1>
  </header>
  <main>
    <div class="wallet-section">
      <h2>Current Balance: ₹{{currentBalance}}</h2>
      <button id="withdrawButton">Withdraw</button>
    </div>
    <div class="withdrawal-form" hidden>
      <h3>Withdrawal Request</h3>
      <form action="/withdraw" method="post">
        <label for="amount">Amount to Withdraw:</label>
        <input type="number" id="amount" name="amount" placeholder="Enter amount" required>
        <label for="paymentMethod">Payment Method:</label>
        <select id="paymentMethod" name="paymentMethod">
          <option value="bank-transfer">Bank Transfer</option>
          <option value="paypal">PayPal</option>
          <option value="cryptocurrency">Cryptocurrency</option>
        </select>
        <button type="submit">Request Withdrawal</button>
        <button type="button" id="cancelWithdrawal">Cancel</button>
      </form>
    </div>
  </main>
  <footer>
    <p>Copyright &copy; 2023</p>
  </footer>
</body>
</html>








<div class="transaction-history">
  <h2>Transaction History</h2>
  <table>
    <thead>
      <tr>
        <th>Date</th>
        <th>Amount</th>
        <th>Payment Method</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>2023-07-20</td>
        <td>₹500</td>
        <td>Bank Transfer</td>
      </tr>
      <tr>
        <td>2023-07-15</td>
        <td>₹1000</td>
        <td>PayPal</td>
      </tr>
    </tbody>
  </table>
</div>



<div class="account-settings">
  <h2>Account Settings</h2>
  <form action="/account-settings" method="post">
    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" placeholder="Enter email address" required>
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" placeholder="Enter password" required>
    <label for="phone-number">Phone Number:</label>
    <input type="tel" id="phone-number" name="phone-number" placeholder="Enter phone number" required>
    <button type="submit">Save Changes</button>
  </form>
</div>




<div class="withdrawal-limits">
  <h2>Withdrawal Limits</h2>
  <p>The minimum withdrawal amount is ₹100. The maximum withdrawal amount is ₹10,000 per day. Withdrawals are processed within 24 hours.</p>
</div>
