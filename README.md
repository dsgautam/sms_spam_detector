# sms_spam_detector
Module 21 Homework Challenge

# Background:
You'll be refactoring code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model. Once the model is created and trained, you will create a Gradio app to host the application, enabling users to test text messages. The application will provide feedback to users, indicating whether the text is classified as spam or not, based on the model's performance.

The data for this exercise is provided and stored in the resources folder: "SMSSpamCollection.csv"

# Solution: 
The solution is included in the github directory "https://github.com/dsgautam/sms_spam_detector"

The solution was developed using Jupyter Notebook , but can be used in Google Colab as well.

The steps taken are broadly defined here:

1. Include module dependencies
2. Read the data into a dataframe from the CSV
3. Define a function (sms_classification) that receives the dataframe as an input parameter
    
    -Map features "text_message" column into X
    
    -Map target "label" into y
    
    -Split Data into Train and Test
    
    -Build a pipeline using appropriate parameters
    
    -Fit the model
    
    -Return the results of the model
4. Define a function (sms_prediction) that receives the user text as an input parameter
    
    -Use the trained model to predict whether the input "text" is a spam or ham
    
    -Return a relevant text message based on the prediction
5. Use Gradio to build a simple user interface
    
    -Receive input text that should be evaluated or test for Spam or Ham
    
    -Send output message whether the input "text" is claissfied as "Spam" or "not Spam"


# Results: 
After executing the Gradio application, the testings results correctly predicted whether the input text is a "spam" or "not spam" 

Live URL generated using Google Colab is https://3bc20353542b211f2d.gradio.live/

This share link expires in 72 hours.