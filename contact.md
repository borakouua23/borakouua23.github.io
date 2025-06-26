<form action="https://formsubmit.co/neshappens@gmail.com" method="POST">
  <h2>Contact Us</h2>

  <label for="name">Name</label><br>
  <input id="name" type="text" name="name" required placeholder="Your Name"><br><br>

  <label for="email">Email</label><br>
  <input id="email" type="email" name="email" required placeholder="Your Email"><br><br>

  <label for="message">Message</label><br>
  <textarea id="message" name="message" required placeholder="Your Message"></textarea><br><br>

  <!-- Disable CAPTCHA -->
  <input type="hidden" name="_captcha" value="false">

  <!-- Redirect to your own Docsify page after submit -->
  <input type="hidden" name="_next" value="https://borakouua23.github.io/#/form/email-sent">

  <button type="submit">Send</button>
</form>
