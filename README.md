# krishnamoorthy19

                     WHATSAPP CHATBOT DEVELOPEMENT USING PYTHON(PYCHARM) 
                     
import pywhatkit as kit
import time

# Function to send a message 
def send_message(phone_number,message,time_hour,time_minutes):

  try:
      kit.sendwhatmsg(phone_number,message,time_hour,time_minutes)
      print("Message sent successfully!")

  except Exception as e:
      print("Error:", str(e))

# Main function 
if __name__ =="__main__":
      phone_number = input("Enter the phone number (with country code) to send the message:")
      message = input("Enter the message to send:")
      time_hour = int(input("Enter the hour to send  the message (24 hour format):"))
      time_minute = int(input("Enter the minute to send the message:"))

      send_message(phone_number,message,time_hour,time_minute)



# output 

Enter the phone number (with country code) to send the message:+91 1236549777
Enter the message to send:HOW ARE YOU
Enter the hour to send  the message (24 hour format):23
Enter the minute to send the message:37
In 50 Seconds WhatsApp will open and after 15 Seconds Message will be Delivered!
Message sent successfully!

Process finished with exit code 0
      
