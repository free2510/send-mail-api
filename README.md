# Sending Emails with URL Parameters using EmailJS

This HTML file demonstrates how to send emails using EmailJS by passing parameters through the URL. This setup allows you to integrate email functionality into web applications without server-side scripting.

## How It Works

### HTML File Explanation

The provided HTML file (`index.html`) includes:

- **EmailJS SDK**: The SDK is included from EmailJS CDN (`https://cdn.emailjs.com/dist/email.min.js`) to facilitate email sending.
  
- **JavaScript Functions**:
  - `getQueryParams()`: Parses URL parameters (`to`, `subject`, `message`) using `URLSearchParams`.
  - `sendEmail()`: Retrieves parameters, validates them, constructs template parameters, and sends an email using EmailJS.
  
- **Send Email Functionality**: When the page loads (`window.onload`), it automatically triggers the `sendEmail()` function, sending an email based on URL parameters.

### How to Use

1. **Include EmailJS SDK**: Ensure the `<script>` tag for EmailJS SDK is present in your HTML file.

2. **Modify Email Template**: Replace `"service_vwyinve"`, `"template_y6ti71u"`, and `"46kPHVk2Hlf0ZuJ5s"` with your actual EmailJS Service ID, Email Template ID, and User ID respectively. These can be obtained from your EmailJS account.

3. **Pass Parameters in URL**:
   - Use the following format to pass parameters:
     ```
     index.html?to=recipient@example.com&subject=Your%20Subject&message=Your%20Message%20Here
     ```
   - Replace `recipient@example.com`, `Your%20Subject`, and `Your%20Message%20Here` with the recipient's email address, subject, and message respectively. Note that spaces are URL-encoded as `%20`.

4. **Send Email**: Open the URL with the parameters in a web browser or programmatically redirect to it from your application to automatically trigger the email sending process.

### Example

To send an email, visit:
index.html?to=recipient@example.com&subject=Welcome&message=Hello%20from%20Our%20Company


This will send an email to `recipient@example.com` with the subject "Welcome" and the message "Hello from Our Company".

### Notes

- Ensure that your EmailJS account is set up correctly with the appropriate service, template, and user IDs.
- Handle security considerations when passing sensitive information through URL parameters.

## License

This code is licensed under the MIT License. See LICENSE file for more details.
