# pythonemail
A Python Function that sends a Email using your Gmail account with a Function using SMTP.



#Send Email
import smtplib

def sendEmail():
    #create object in this case we User GMAIL , 587 is Gmail.
    smtpObj = smtplib.SMTP('smtp.gmail.com', 587)
    #Encryption.
    smtpObj.starttls()
    #Time to login to your email, then enter your password.
    smtpObj.login(' youremail@gmail.com', 'passwordhere')
    #Now Create your Message remember to add your email, then receivers email, subject, message.
    smtpObj.sendmail(' youremail@gmail.com', 'receiversemail@gmail.com',
		 'Subject: How you been., Remember me,')
