<form action="https://formsubmit.co/neshappens@gmail.com" method="POST">
  <input type="text" name="name" placeholder="Your Name" required>
  <input type="email" name="email" placeholder="Your Email" required>
  <textarea name="message" placeholder="Your Message" required></textarea>

  <!-- Disable CAPTCHA -->
  <input type="hidden" name="_captcha" value="false">

  <!-- Redirect to your own Docsify page after submit -->
  <input type="hidden" name="_next" value="https://borakouua23.github.io/#/form/email-sent">

  <button type="submit">Send</button>
</form>
