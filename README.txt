Alexa Source Files:

	Skillbuilder.json
	
		This file maps the user's utterances to Intents.  The Intents get sent to the AWS Lambda function for processing.
		
	ZAdventure.java
		Defines the ZAdventure object; how the Adventure gets stored in Firebase.
	
	ZEvent.java	
		Defines the ZEvent object; how Events gets stored in Firebase.
	
	ZLinkRequest.java
		Defines the ZLinkRequest object; how a request to link the Alexa account with an Android account is stored in Firebase.
		
	LambdaFunctionHandler.java
		The AWS lamdbda function entry point
		Calls ACSpeechlet.java to do the actual processing
	
	ACSpeechlet.java	
		The main Alexa processing function file; it responds to the user's Intents and runs the adventures.
		
		

Maven instructions for Alexa Skill:

	cd into the project directory (adventure_creator_skill/)

	from the command line type: mvn install
	
	this will pull all of the dependencies you need to compile
	
	then run the command: mvn clean package

	this will compile the Java files and give you ouput in the terminal
	and will also build your JAR files

	Here is a link to Maven if you don't have it installed already

	https://maven.apache.org/download.cgi
	

