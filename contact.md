<form id="contact-form">
  <input type="text" name="name" placeholder="Your Name" required>
  <input type="email" name="email" placeholder="Your Email" required>
  <textarea name="message" placeholder="Your Message" required></textarea>
  <!-- Disable CAPTCHA -->
  <input type="hidden" name="_captcha" value="false">
  <button type="submit">Send</button>
</form>

<script>
  document.getElementById('contact-form').addEventListener('submit', function(e) {
    e.preventDefault(); // stop default redirect

    const form = e.target;
    const data = new FormData(form);

    fetch('https://formsubmit.co/ajax/neshappens@gmail.com', {
      method: 'POST',
      body: data,
      headers: { 'Accept': 'application/json' }
    })
    .then(response => {
      if (response.ok) {
        alert('✅ Mail sent successfully!');
        form.reset();
      } else {
        return response.json().then(json => {
          throw new Error(json.message || 'Submission failed.');
        });
      }
    })
    .catch(err => {
      alert('⚠️ Error: ' + err.message);
    });
  });
</script>
