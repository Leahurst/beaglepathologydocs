#Emailing from Beagle
**This documentation should be replaced with a pointer to the equivalent documentation in Beagle Core once the functionality has been added to Core.**

##Overview
The Beagle code contains a function which handles emailing. That function accepts parameters such as the recipient, the subject, the content, any attachments and so on. The function is called whenever the option is to email a document is triggered by a User, e.g. when clicking the button to email an Invoice or a Report.

Due to issues with passing the application User's credentials to the Exchange server (the 'double hop' problem), all emails from Beagle are sent from a predefined Beagle account, specified in the System Configuration table. Before a User can send emails from Beagle, they must grant that account Delegate permissions to their Exchange mailbox so that the Beagle account can 'send on behalf of' the User.