Using Amazon DynamoDb database in Amazon Lambda function, implemented on Java, for AWS Lex bot.

Demo project for the introduction video tutorial: https://youtu.be/cy9GX33nuKM

See also: "Tutorial: AWS Lambda function for Amazon Lex; Implemented on Java": https://youtu.be/HkMi5xPyz1g

Amazon Lex allows to build conversation bots and integrate them to Facebook Messenger, Slack or Twilio: https://aws.amazon.com/lex/

AWS Lambda a set of functions and components, which can be implemented on different runtimes - Node, Java, C#, Python: https://aws.amazon.com/lambda/

1. Create a group with needed access in IAM: https://console.aws.amazon.com/iam/home#/groups
2. Create a user: https://console.aws.amazon.com/iam/home#/users
3. Add the created user to the created group: https://console.aws.amazon.com/iam/home#/users/user1?section=groups
4. Setup credentials on the local computer: http://docs.aws.amazon.com/sdk-for-java/v1/developer-guide/setup-credentials.html
Credentials will be stiored in the file:
```
~/.aws/credentials
[default]
aws_access_key_id = …
aws_secret_access_key = …
```
4. For local testing - install DynamoDBLocal
https://github.com/awslabs/aws-dynamodb-examples/blob/master/src/test/java/com/amazonaws/services/dynamodbv2/DynamoDBLocalFixture.java
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.html

Java SDK:
```
aws-java-sdk-lambda
aws-lambda-java-core
aws-java-sdk-dynamodb
dexmaker-mockito
```
Developer Guide:  
https://aws.amazon.com/documentation/dynamodb
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide

Introduction and design: 
https://www.slideshare.net/AmazonWebServices/design-patterns-using-amazon-dynamodb
https://www.youtube.com/watch?v=XByPxb_VvpY&t=796s

Work with tables: 
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/JavaDocumentAPITablesExample.html

DynamoDBMapper: 
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBMapper.html
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/QueryingJavaDocumentAPI.html
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ScanJavaDocumentAPI.html
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBMapper.QueryScanExample.html

CRUD operations: 
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/JavaDocumentAPICRUDExample.html

Other: 
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GuidelinesForItems.html
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.NamingRulesDataTypes.html
http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBMapper.ArbitraryDataMapping.html
