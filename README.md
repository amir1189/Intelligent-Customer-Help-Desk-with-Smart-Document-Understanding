Intelligent Customer helpdesks with Smart Document Understanding

Internship Title : Intelligent Customer Help Desk with Smart Document Understanding-SB48559
                                      
This is repository build with the help of Watson Assistant, Discovery, Cloud Function and Node Red app of IBM Cloud. It is made with the
regard of partial fulfillment of Smartinternz Internship Program at smartbrigde.

Project Description :
The typical customer care chatbot can answer simple questions, such as store locations and hours, directions, and 
maybe even making appointments. When a question falls outside of the scope of the pre-determined question set, the option is typically to
tell the customer the question isn’t valid or offer to speak to a real person.

Solution Description :
In this project, there will be another option. If the customer question is about the operation of a device, the application shall pass the 
question onto Watson Discovery Service, which has been pre-loaded with the device’s owners manual. So now, instead of “Would you like to 
speak to a customer representative?” we can return relevant sections of the owners manual to help solve our customers’ problems. To take 
it a step further, the project shall use the Smart Document Understanding feature of Watson Discovery to train it on what text in the 
owners manual is important and what is not. This will improve the answers returned from the queries. Scope of Work Create a customer care 
dialog skill in Watson Assistant Use Smart Document Understanding to build an enhanced Watson Discovery collection Create an IBM Cloud 
Functions web action that allows Watson Assistant to post queries to Watson Discovery Build a web application with integration to all 
these services & deploy the same on IBM Cloud Platform.
In Watson Discovery I have added VU43 Television User manual.

Project Requirements:GitHub account,Slack App,Python, IBM Cloud Platform,IBM Watson Services,IBM Cloud functions.

Project Deliverables:

1.Create a customer care dialog skill in Watson Assistant
2.Use Smart Document Understanding to build an enhanced Watson Discovery collection
3.Create an IBM Cloud Functions web action that allows Watson Assistant to post queries to Watson Discovery
4.Build a web application with integration to all these services & deploy the same on IBM Cloud Platform

What is SDU?

SDU trains Watson Discovery to extract custom fields in your documents. Customizing how your documents are indexed into Discovery will
improve the answers returned from queries.
With SDU, you annotate fields within your documents to train custom conversion models. As you annotate, Watson is learning and will 
start predicting annotations. SDU models can also be exported and used on other collections.

What is a webhook?

A webhook is a mechanism that allows you to call out to an external program based on something happening in your program. When used in 
a Watson Assistant dialog skill, a webhook is triggered when the Assistant processes a node that has a webhook enabled. The webhook 
collects data that you specify or that you collect from the user during the conversation and save in context variables, and sends the 
data to the Webhook request URL as an HTTP POST request. The URL that receives the webhook is the listener. It performs a predefined 
action using the information that is provided by the webhook as specified in the webhook definition, and can optionally return a 
response.

In our project,the webhook will communicate with an IBM Cloud Functions web action, which is connected to the Watson Discovery service.
1.The document is annotated using Watson Discovery SDU
2.The user interacts with the backend server via the app UI. The frontend app UI is a chatbot that engages the user in a conversation.
3.Dialog between the user and backend server is coordinated using a Watson Assistant dialog skill.
4.If the user asks a product operation question, a search query is passed to a predefined IBM Cloud Functions action.
5.The Cloud Functions action will query the Watson Discovery service and return the results.

Node-Red Dashboard link after deploying :https://node-red-grfzx.eu-gb.mybluemix.net/ui

Youtube video links :-

Demonstration Video: https://youtu.be/4OsPazUG0ac
Feedback Video: https://youtu.be/plcFjHN4U5I
