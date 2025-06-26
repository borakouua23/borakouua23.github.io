# reess4
gsx

<form id="contactForm" action="https://formsubmit.co/sssssssssssss@gmail.com" method="POST">
  <label for="name">Name:</label>
  <input type="text" name="name" required><br><br>

  <label for="email">Email:</label>
  <input type="email" name="email" required><br><br>

  <label for="message">Message:</label><br>
  <textarea name="message" rows="5" required></textarea><br>

  <input type="hidden" name="_captcha" value="false">

  <button type="submit">Send</button>
</form>

<script>
  document.getElementById("contactForm").addEventListener("submit", function (e) {
    e.preventDefault(); // prevent default form submission

    // Create and append _next input
    const nextInput = document.createElement("input");
    nextInput.type = "hidden";
    nextInput.name = "_next";
    nextInput.value = window.location.origin + "/#/email-sent";

    this.appendChild(nextInput);

    // Submit the form manually after adding the hidden input
    this.submit();
  });
</script>
