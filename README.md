This project aims to develop an automatic spam tagging system using cloud computing and big data technologies. The system will be able to classify incoming emails as spam or not spam in real-time, using a machine learning model trained on SMS message data.

The project has several components. First, we will complete a tutorial for using Amazon SageMaker on AWS, which will familiarize us with the basic components of SageMaker. Next, we will implement a machine learning model for predicting whether an SMS message is spam or not, following an AWS tutorial on building and training a spam filter machine learning model using Amazon SageMaker.

Once the machine learning model is trained and performs well on emails, we will deploy the resulting model to an endpoint. We will then create an S3 bucket to store incoming email files and use SES to set up an email address that, upon receipt of an email, will store it in S3. For any new email file that is stored in S3, we will trigger a Lambda function that extracts the body of the email and uses the prediction endpoint to predict if the email is spam or not. We will then reply to the sender of the email with a message indicating whether the email is spam or not, and the confidence score of the classification.

Finally, we will create an AWS CloudFormation template for the automatic spam tagging system. The template will represent all the infrastructure resources and permissions required for the system, such as Lambda, SES configuration, IAM policies, roles, and the prediction endpoint as a stack parameter.

The project's success criteria will be based on the system's ability to accurately classify incoming emails as spam or not spam in real-time. We will also test the CloudFormation template and ensure that it can be used to set up the system in a separate account with a different prediction endpoint.

Overall, this project aims to leverage cloud computing and big data technologies to develop an automatic spam tagging system that can provide efficient and accurate email filtering. The project's outcome can have practical applications in various domains, including e-commerce, social media, and telecommunications, where spam filtering is a critical issue.



<img width="1105" alt="image" src="https://user-images.githubusercontent.com/97984259/230731876-77e47579-cf7c-4531-95a3-eda0dbc142fc.png">

