# WikiBreach

Executing this will let you populate a database with meta-data of cyberbreaches extracted from the web, in the form of json strctured files.
Gmail API authenticates a gmail account which gets Google Alerts about cyberbreaches. 
API list messages call gives the message IDs for each email. This message ID is used to extract the content of the entire email using API 
get message call. 
The message has to be decoded from base64 url to utf-8.
The extracted url of article is sent to Diffbot using Diffbot Article API and their developer token to get meta-data related to article. 

As soon as the code loads, it authenticates the gmail account and parses it. Then click on the Diffbot Request button to send urls to 
Diffbot. Then click on Download Response to have a json file of meta-data of all articles. 
