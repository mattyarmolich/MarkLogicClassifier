Mark Logic Classifier Front End

To install the front end

0. ensure you have the appropriate version of yarn or npm

1. Clone the repo from https://github.com/mattyarmolich/MarkLogicClassifier.git using the command
'git clone https://github.com/mattyarmolich/MarkLogicClassifier.git'

2. cd into the directory

3. run yarn/npm install to load all of the external depencencies of the project

4A. - if running locally install the CORS allow plugin for chrome to allow external GET/POST requests to function as if its been deployed
	- run yarn start to run locally 
	- configure the urlAssets file in /utils to hit your desired endpoint link for the backend
	
4B. to deploy to s3 use the amazon aws cli with s3
	- create an s3 bucket with public policy and public access
	- setup the AWS CLI using aws configue and entering in your secret credentials
	- run yarn run build && yarn deploy to deploy to that s3 bucket
	- access the code through your buckets link
