Instructions for setting up sample implementation:

1. How reader can setup example on their local machine. 
	 	- Reader will create an account on Glitch.com and LaunchDarkly.com if they don't already have one. 
	 	- In Glitch, the user will select 'New Project' in upper right-hand corner and then choose 'Import from GitHub' at the very bottom. This will allow the 			new user to import the contents of this repo to view and start using the Web app in Glitch. 
	 
2. Setting up LaunchDarkly SDK
		- Create a new Project in LaunchDarkly using a client-side SDK. We will be working with a Python SDK.
		- Copy the SDK key from the Production environment. This is what will be stored in an environment variable within the application.
		- In Glitch, the .env file will require a variable called LD_SDK_KEY and assign the value of the SDK key you copied here. 
		- If you look in the requirements file, you will find that the launchdarkly-server-sdk is already listed as a dependency to the Python app.
		
3. Creating Feature Flag
		- User will re-create the feature flag called Pricing tier 3 along with the targeting. 
		- Under 'Target Users who match these rules' emails that start with 'a' or 'A' will serve a value of 'True' and be able to view the third pricing tier. 
		- Default rule will be set to False.
