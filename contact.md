<form 
  action="https://formsubmit.co/neshappens@gmail.com" 
  method="POST"
>
  <!-- Form Fields -->
  <input type="text" name="name" placeholder="Your Name" required>
  <input type="email" name="email" placeholder="Your Email" required>
  <textarea name="message" placeholder="Your Message" required></textarea>

  <!-- Hidden Inputs -->
  <input type="hidden" name="_captcha" value="false">
  <input type="hidden" name="_redirect" id="redirect-input">

  <!-- Submit -->
  <button type="submit">Send</button>
</form>

<script>
  // Set redirect dynamically based on current domain
  document.addEventListener("DOMContentLoaded", function () {
    const redirectUrl = `${window.location.origin}/#/form/email-sent`;
    document.getElementById("redirect-input").value = redirectUrl;
  });
</script>
