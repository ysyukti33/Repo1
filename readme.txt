These are changes regarding XCE-1630, XCE-2228 and .sh file of OCR

Sources Details and Release Path:
Release Path:
	BitBucket repo: https://bitbucket.pvai.com/projects/PVAI/repos/cora-ai-pvai-rage/
	BitBucket Branch: release/2.0C
	Folder Name : ExtractionObject_LearningStore_changes

1. Extraction_Object Sources List:-
	a. sr3_xce_Services-0.0.1-SNAPSHOT-jar-with-dependencies.jar
	b. config.properties
	c. lib

2. Learning_Store Sources List:-
	a. RageLearningStore-1.0-jar-with-dependencies.jar
	b. config.properties
	

Deployment steps:
1. Extraction Object Sources Deployment:-
	a. First navigate to the /opt/application/wildfly-10.1.0.Final/ci/ExtractionObject path
	b. Take back up of existing sr3_xce_Services-0.0.1-SNAPSHOT-jar-with-dependencies.jar, config.properties and lib folder.
	c. Copy the sources sr3_xce_Services-0.0.1-SNAPSHOT-jar-with-dependencies.jar, config.properties and lib folder from release path 
	    to /opt/application/wildfly-10.1.0.Final/ci/ExtractionObject
	d. Replace the DB properties from config.properties according to the environment.
	e. testing file

2. Learning Store Sources Deployment:-
	a. First navigate to the /opt/application/wildfly-10.1.0.Final/ci/LearningStore path
	b. Take the back up of existing RageLearningStore-1.0-jar-with-dependencies.jar, config.properties.
	c. Copy the sources RageLearningStore-1.0-jar-with-dependencies.jar, config.properties from release path to path 
	   /opt/application/wildfly-10.1.0.Final/ci/LearningStore and /opt/application/wildfly-10.1.0.Final/ci/LearningStore/resources/.
	d. Please ensure to change the S3 bucket name(learning.s3.bucketName), 
	S3 access key(learning.s3.accessKey) and S3 secret key(learning.s3.secretKey) in config.properties file according to environment.

3. Test converter file:-
	a. Tracking files

