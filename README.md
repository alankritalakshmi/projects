[Chatbot for Ordering Starbucks](https://bot.dialogflow.com/069e7547-b6c7-435b-b881-c276edce665c)

# Overview:
This is an attempt to create a no-code chatbot for ordering coffee from Starbucks using Google Dialogflow. The chatbot starts by asking the user for a six-digit pincode to locate the nearest store, and proceeds to ask three things asked by employees at almost all Starbucks outlets: the size of the drink, the name of the drink, and if the customer would like the beverage hot or cold. 

# Setting of Intent:
Started by setting up a default intent with the following set of user prompts:

<img width="446" alt="Screenshot 2022-10-16 161510" src="https://user-images.githubusercontent.com/53871648/196031080-eccab09c-a996-454d-8b12-319ef8e74d0f.png">

After giving user prompts, the following text responses were also fed to the chatbot as part of the training phrases:

<img width="659" alt="Screenshot 2022-10-16 162145" src="https://user-images.githubusercontent.com/53871648/196031302-c939cc3b-689b-4c9b-b72f-d27de53df5a5.png">

After setting up the default welcome intent, some follow-up intent was added to ask for more data from the user - as soon as the chatbot is triggered, it first asks the user for their pincode or zipcode to locate the nearest Starbucks outlet for delivery. The user responses for this are as follows:

<img width="440" alt="Screenshot 2022-10-16 162940" src="https://user-images.githubusercontent.com/53871648/196031609-ecf83282-3f91-43fb-9e88-885ab7d6a9f8.png">

The following actions and parameters were added: apart from the zipcode which is a number entity, the size, temperature, and name of the drink are added as some more parameters with a sys.any type of entity:

<img width="634" alt="Screenshot 2022-10-16 163340" src="https://user-images.githubusercontent.com/53871648/196031749-37071e99-dc76-4fcf-b2c5-e04cb9b104eb.png">

Additional prompts are added for each of these parameters:
For the size:

<img width="728" alt="Screenshot 2022-10-16 163511" src="https://user-images.githubusercontent.com/53871648/196031803-e1cd7a18-f8be-4a7f-8168-11d10fe427df.png">

For the name of the drink:

<img width="600" alt="Screenshot 2022-10-16 163631" src="https://user-images.githubusercontent.com/53871648/196031840-59672f92-f576-45a9-b35a-15f9c02952be.png">

For the temperature, the user is offerred a choice between a hot or an iced drink:


<img width="609" alt="Screenshot 2022-10-16 163738" src="https://user-images.githubusercontent.com/53871648/196031877-336b633d-838e-4e8f-bbd8-c04790bc89fb.png">




