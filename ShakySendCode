# Check Read me on how to install smtplib
import smtplib
from email.message import EmailMessage

# To[Person you're sending email to], subject[Subject of the email], body[Context of the email].
def shakySend(to, subject, body):
    ping = EmailMessage()
    ping.set_content(body)
    ping['subject'] = subject
    ping['to'] = to

    # Enter your email in here bro..
    user = "Email Goes Here"
    ping['from'] = user
    # This is where you get your app password from gmail.
    password = "Password Goes here"

    bot = smtplib.SMTP("smtp.gmail.com", 587)
    bot.starttls()
    bot.login(user, password)
    bot.send_message(ping)

    bot.quit()


if __name__ == '__main__':
    # To, subject, body. [def shakySend(to, subject, body):]
    shakySend("--To--", "--Subject--", "--body--")
