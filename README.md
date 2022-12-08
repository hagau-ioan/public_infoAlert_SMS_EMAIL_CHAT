# public_infoAlert_SMS_EMAIL_CHAT
Automation delivery messages system to send Email/SMS/Chat messages to clients.

# Short summary

The project is built using:

- Kotlin
- Hilt
- Retrofit
- coroutines
- RX
- LiveData
- combination of Alarm Manager and Workmanager. 
- Client flavors
- MVVM + Layer Architectures
- ViewBinding
- etc ...

A microservice/email service handler written in php  was built to send the information collected from Google cloud back to the app and also to react at the app requests to send emails or chat messages.
The email sending process is built on the server side.
Why Google Cloud? Easier to extend  the rights for some resources to more clients because many of them have @gmail.com address and is very flexible and simple to be used. 

# About the App
The goal of this app was to import a list of messages from google cloud xls file, prepaired by the clients and to send these messages/events using the app regulary.
After the list is imported into the app (because the client requested this, the process is done manually by pressing a button "Import" in the app) a background process is setup and regular checks and send/receive operations are done in background. 
Even the app is closed, phone is restarted the background process will continue to work and to send the messages/events if there are any. 
Because the most modern libraries and tools were used from Android world the battery of the device is used at the minimal.

# Screenshots of the app

##### Login Screen.
![alt text](https://roomwizard.hagau.ro/alert-info-screens/info_alert_s5.png)
