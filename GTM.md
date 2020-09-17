
open modal waitlist []
  (click) button#waitlist-modal-open

submit btn modal waitlist []
  (click) input#mc-embedded-subscribe.modalSubmitBtn

form submission failure modal waitlist []

  (visible) .modal-body #mce-error-response.form-submit-failure

form submission success modal waitlist []
  (visible) .modal-body #mce-success-response.form-submit-success

close modal waitlist
  (click) button#waitlistModalCloseBtn

click submit btn on page waitlist []
  (click) input#mc-embedded-subscribe.onPageSubmitBtn

waitlist on page form submission failure []
  (visible) #mc_embed_on_page_wrapper #mce-success-response.form-submit-success

waitlist on page form submission success []
  (visible) #mc_embed_on_page_wrapper #mce-error-response.form-submit-failure

scroll depth [X]



Google Analytics by default stores a new Client Id in cookies. Across devices, new clientId's are generated so user John, could have client id 1 for his laptop, client id 2 for his phone, and client id 3 for desktop.

The way to get around this is by using a userId inside Google Analytics and GTM.

https://www.analyticsmania.com/post/google-analytics-user-id-with-google-tag-manager/


if agree to cookies
 store userId []
 store consent boolean true []

 if disagree to cookies
  store userId []
  store consent boolean false []
