---
layout: default
title: Contact Us
permalink: /contact/
---

# Contact Us

Have feedback or questions? We'd love to hear from you!

<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="contact-form">
  <div class="form-group">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" required placeholder="Your name" class="form-control">
  </div>

  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" id="email" name="email" required placeholder="your.email@example.com" class="form-control">
  </div>

  <div class="form-group">
    <label for="subject">Subject</label>
    <input type="text" id="subject" name="subject" required placeholder="Brief subject" class="form-control">
  </div>

  <div class="form-group">
    <label for="message">Message</label>
    <textarea id="message" name="message" rows="6" required placeholder="Your message here..." class="form-control"></textarea>
  </div>

  <!-- Honeypot field for spam protection -->
  <input type="text" name="_gotcha" style="display:none">

  <!-- Formspree configuration -->
  <input type="hidden" name="_subject" value="New contact form submission">
  <input type="hidden" name="_next" value="{{ '/contact-thank-you' | absolute_url }}">

  <button type="submit" class="btn btn-primary">Send Message</button>
</form>

---

*Your privacy is important. This form is handled securely by [Formspree](https://formspree.io/).*
