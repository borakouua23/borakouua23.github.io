<form 
  action="https://formsubmit.co/neshappens@gmail.com" 
  method="POST"
>
  <input type="text" name="name" required placeholder="Your Name">
  <input type="email" name="email" required placeholder="Your Email">
  <textarea name="message" required placeholder="Your Message"></textarea>

  <!-- CAPTCHA off -->
  <input type="hidden" name="_captcha" value="false">

  <!-- Set dynamically -->
  <input type="hidden" name="_redirect" id="redirect-input">

  <button type="submit">Send</button>
</form>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const redirectUrl = `${window.location.origin}/#/form/email-sent`;
    document.getElementById("redirect-input").value = redirectUrl;
  });
</script>
