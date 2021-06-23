<script>

  let mail = {
    name: "",
    email: "",
    phoneNumber: "",
    subject: "",
    message: "",
  };

  const handleSubmit = (e, mail) => {
    e.preventDefault();
    e.stopPropagation()
    console.log(mail)
  };
</script>


<!-- CONTACT FORM : begin -->
<form on:submit={(e) => handleSubmit(e, mail)}>
  
  <div class="row">
    <div class="col-sm-4">
      <!-- NAME FIELD : begin -->
      <div class="form-field">
        <label for="contact-name">Your Name <span>*</span></label>
        <input name="contact-name" bind:value={mail.name} class="m-required" />
      </div>
      <!-- NAME FIELD : end -->

      <!-- EMAIL FIELD : begin -->
      <div class="form-field">
        <label for="contact-email">Your Email Address <span>*</span></label>
        <input
          name="contact-email"
          bind:value={mail.email}
          class="m-required m-email"
        />
      </div>
      <!-- EMAIL FIELD : end -->

      <!-- PHONE FIELD : begin -->
      <div class="form-field">
        <label for="contact-phone">Your Phone Number</label>
        <input name="contact-phone" bind:value={mail.phoneNumber} />
      </div>
      <!-- PHONE FIELD : end -->
    </div>
    <div class="col-sm-8">
      <!-- SUBJECT FIELD : begin -->
      <div class="form-field">
        <label for="contact-subject">Message Subject</label>
        <input name="contact-subject" bind:value={mail.subject} />
      </div>
      <!-- SUBJECT FIELD : end -->

      <!-- MESSAGE FIELD : begin -->
      <div class="form-field">
        <label for="contact-message">Message <span>*</span></label>
        <textarea
          name="contact-message"
          bind:value={mail.message}
          class="m-required"
        />
      </div>
      <!-- MESSAGE FIELD : end -->

      <!-- SUBMIT BUTTON : begin -->
      <div class="form-field">
        <button
          class="submit-btn c-button"
          type="submit"
          data-label="Send Message"
          data-loading-label="Sending...">Send Message</button
        >
      </div>
      <!-- SUBMIT BUTTON : end -->
    </div>
  </div>
</form>
<!-- CONTACT FORM : end -->

<style>
form input, form textarea {
  background-color: #f1f1f1;
  color:#696969;
  display:inline-block;
  flex-direction:column;
  font-family: Source Sans Pro;
  font-weight: 300;
  padding: 13px 15px;
  width: 100%
}

textarea {
  min-height: 150px;
  margin-bottom: .5rem;
}
</style>
