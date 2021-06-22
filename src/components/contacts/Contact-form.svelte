<!-- CONTACT FORM : begin -->
    <form
      id="contact-form"
      class="default-form m-ajax-form"
      action="ajax/contact-form.php"
      method="post"
    >
      <input type="hidden" name="contact-form" />

      <!-- FORM VALIDATION ERROR MESSAGE : begin -->
      <p
        class="c-alert-message m-warning m-validation-error"
        style="display: none;"
      >
        <i class="ico fa fa-exclamation-circle" />Please fill in all required
        (*) fields.
      </p>
      <!-- FORM VALIDATION ERROR MESSAGE : end -->

      <!-- SENDING REQUEST ERROR MESSAGE : begin -->
      <p
        class="c-alert-message m-warning m-request-error"
        style="display: none;"
      >
        <i class="ico fa fa-exclamation-circle" />There was a connection
        problem. Try again later.
      </p>
      <!-- SENDING REQUEST ERROR MESSAGE : end -->

      <div class="row">
        <div class="col-sm-4">
          <!-- NAME FIELD : begin -->
          <div class="form-field">
            <label for="contact-name">Your Name <span>*</span></label>
            <input id="contact-name" name="contact-name" class="m-required" />
          </div>
          <!-- NAME FIELD : end -->

          <!-- EMAIL FIELD : begin -->
          <div class="form-field">
            <label for="contact-email">Your Email Address <span>*</span></label>
            <input
              id="contact-email"
              name="contact-email"
              class="m-required m-email"
            />
          </div>
          <p style="display: none;">
            <label for="contact-email-hp">Re Email Address</label>
            <input id="contact-email-hp" name="contact-email-hp" />
          </p>
          <!-- EMAIL FIELD : end -->

          <!-- PHONE FIELD : begin -->
          <div class="form-field">
            <label for="contact-phone">Your Phone Number</label>
            <input id="contact-phone" name="contact-phone" />
          </div>
          <!-- PHONE FIELD : end -->
        </div>
        <div class="col-sm-8">
          <!-- SUBJECT FIELD : begin -->
          <div class="form-field">
            <label for="contact-subject">Message Subject</label>
            <input id="contact-subject" name="contact-subject" />
          </div>
          <!-- SUBJECT FIELD : end -->

          <!-- MESSAGE FIELD : begin -->
          <div class="form-field">
            <label for="contact-message">Message <span>*</span></label>
            <textarea
              id="contact-message"
              name="contact-message"
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