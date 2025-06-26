# ree

<form action="https://formsubmit.co/receiver_email@gmail.com" method="POST">
  <label for="name">Name:</label>
  <input type="text" name="name" required><br><br>
  <label for="email">Email:</label>
  <input type="email" name="email" required><br><br>
  <label for="message">Message:</label><br>
  <textarea name="message" rows="5" required></textarea><br>
   <input type="hidden" name="_next" value="http://localhost:8000/#/email-sent">
  <input type="hidden" name="_captcha" value="false">
  <button type="submit">Send</button>
</form>
