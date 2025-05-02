used to send emails using the Simple Mail Transfer Protocol (SMTP).

Basic Concepts You Need to Know:
1. SMTP Server
This is the mail server that sends your email to the recipient.
For Gmail, the SMTP server is: smtp.gmail.com and the port is 587.

2. Ports
Port 587 is commonly used for sending emails securely using TLS encryption.

3. Login
To send an email, you must login to your email account inside your Python code using your email and App Password (for Gmail).

```python
import smtplib
# email details
sender = "youremail@gmail.com"
password = "your-app-password"
receiver = "receiver@example.com"

# Message Formatting
subject = "Test Email"
body = "This is a simple email"
# Combine subject and body into 1 message
message = f"Subject: {subject}\n\n{body}"

try:
    # Connect to Gmail's SMTP server
    server = smtplib.SMTP_SSL('smtp.gmail.com', 465)
    # Login to Your Email Account
    server.login(sender_email, password)
    # Send the Email
    server.sendmail(sender_email, receiver_email, message)
    #Close the Connection
    server.quit()

    print("Email sent successfully!")
    
except Exception as e:
    print(f"Failed to send email. Error: {e}")
```