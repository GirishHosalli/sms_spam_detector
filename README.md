# SMS Spam Detecor App
This app can be used to detect if a SMS text message is spam. App interface was created using Gradio which has an input and an output boxes.

SMS Classification model is created:
SMS Classification model uses a pipeline with TF-IDF vectorization and Linear Support Vector Classification.

    Parameters
    sms_text_df (pd.DataFrame): DataFrame containing 'text_message' and 'label' columns for SMS classification.
    
    Returns:
    - text_clf (Pipeline): Fitted pipeline model for SMS classification.

    This function takes a DataFrame with 'text_message' and 'label' columns, splits the data into
    training and testing sets, builds a pipeline with TF-IDF vectorization and Linear Support Vector
    Classification, and fits the model to the training data. 
    The fitted pipeline is returned to make future predictions.

Gradio app has -
- Input box with label "What is the test message you want to test?"
- Output box with label "Our app has determined:"
After user inputs the SMS text message in the input box:
- Function "sms_prediction" is called and SMS text message is passed into it
- This function will use a SMS text classification model to predict if the message is a Spam
- This funcrtion will return a text string back to the app indicating if the SMS message is a 'spam' or 'not a spam'

![image](https://github.com/user-attachments/assets/821d48b3-808c-4647-b8da-24d9c3524ee8)

