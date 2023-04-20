# Postman-Collection
This is my postman collection from COLT 01/2023 Cherry IT initiative.
This collection based on Trello board and if u want to run this collection follow this steps.

## Requirements

To use this Postman collection, you need:

- Postman application - you can download it from https://www.postman.com/downloads/
- [Trello](https://trello.com/home) account with created workspace Power up (In iframe connector URL u can use https://my-power-up.com) [Here is a instruction](https://developer.atlassian.com/cloud/trello/guides/rest-api/api-introduction/)
- If you have generated token and key you must add this to collection variables (without this step collection won't run cause of no authorization)

## How to import the Postman collection

1. Save Trello_Requests_Collection.json file: Go to [Trello_Requests_Collection.json file](https://github.com/Kurzydlak/Postman-Collection/blob/main/Postman%20Collections/Trello_Requests_Collection.json).
Click right button on RAW and Save linked file as .json file.

2. Open the Postman application and import the collection by clicking on the "Import" button.
Next navigate to the downloaded file and select it.

## Description of requests in the collection

The Postman collection consists of the following requests:

BOARD:

- 'CREATE A BOARD' - Creating a new board and if Id board is not exist defines it as collection variable.
- 'UPDATE A BOARD' - Updating a board with specific id.
- 'GET A BOARD' - Getting a board with specific id.
- 'DELETE A BOARD'- Deleting board with specific id and deleting every id's which was defined as collection variables in other requests.

LIST:

- 'CREATE NEW LIST' - Creating a new list and if Id List is not exist defines it as collection variable.
- 'GET A LIST' - Getting a list with specific id.
- 'UPDATE A LIST' - Updating a list with specific id.

CARD:

- 'CREATE NEW CARD' - Creating a new card and if Id Card is not exist defines it as collection variable.
- 'GET A CARD' - Getting a card with specific id.
- 'ADD A NEW COMMENT TO A CARD' - Adding a new comment to a card and if Id comment is not exist defines it as collection variable.
- 'DELETE A COMMENT ON A CARD' - Deleting added comment to a card and deleting Id of this comment which was defined as collection variable.
- 'UPDATE A CARD' - Updating a card with specific id.
- 'DELETE A CARD' - Deleting a card and deleting Id of this card which was defined as collection variable.

LABEL:

- 'CREATE NEW LIST' - Creating a new label and if Id Label is not exist defines it as collection variable.
- 'GET A LIST' - Getting a label with specific id.
- 'UPDATE A LIST' - Updating a label with specific id.
- 'DELETE A LABEL' - Deleting a label and deleting Id of this label which was defined as collection variable.

ATTACHMENTS:
- 'CREATE ATTACHMENT ON A CARD - Creating a new attachment and if Id Attachment is not exist defines it as collection variable.
- 'GET AN ATTACHMENT ON A CARD' - Getting an a a attachment with specific id.
- 'DELETE AN ATTACHMENT ON A CARD' - Deleting attachment an and deleting Id of this attachment which was defined as collection variable.

## If you want to run this collection

1. First send a 'GET A BOARD' request and notice a board is not created (if status of response is 400 bad request and test was failed board is not created)
2. Right click on Trello requests in Postman app and choose 'Run collection'
3. Deselect all Delete request and click 'Run Trello Requests.
4. If you want to run this again send a 'DELETE A BOARD' request this will delete a board and clear all setted variables.



