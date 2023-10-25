# Hello! #
If you're looking at this, you're probably considering joining our Infrastructure team as Cloud, DevOps or ML Ops engineer.  We're excited to meet you. Please do not be 
intimidated by
the size of this document.  We do not expect _anyone_ to exceed the recommended maximum time of 2 hours.  There is no minimum 'score' to pass.   This is 
intended to be a challenging technical exercise, but also let you demonstrate to us your ability to identify roadblocks in a reasonable timeframe and communicate how they impact your 
ability to move forward.  Our team is actively working on new technologies within the AWS ecosystem; so there'll be a lot of times where an engineer might not know something. The 
ability to assess, determine a path forward and communicate with the team is a very important skill.  Yes the technical unicorn exists, but purely technical skills aren't the only 
strength an individual brings to the table.

If you get stuck on something, comment on it in the same way you might bring it up to the team during a daily standup.   If any part of this exercise is unclear, please take time
to point it out and what about the question was difficult. If you feel it is taking more time to accomplish than you have to commit, please let us know that as well. Our goal is not to waste anyone's time, 
but to have a rich set of exercises that you can use to demonstrate your skills.

It is a good idea to test what you plan to submit, keep in mind that AWS does provide free accounts that you can use to prepare this exercise.

# Infrastructure As Code #
Much of our work is managing the infrastructure on which we manage our systems. One of our mottos is _Infrastructure as Code_, and to this end, we heavily use AWS CloudFormation, 
Terraform, AWS CLI and AWS CDK.

## CloudFormation ##
Explain how you would use CloudFormation to deploy a web application with auto-scaling, load balancing, and robust security. Provide a sample CloudFormation template snippet demonstrating the following.
- Instantiate a pair of s3 buckets.
- Create and apply a pair of policies, one that sets one of the buckets to be public, the second to be private.
- Create a new user named `vera`.
- Create a `developer` role and make `vera` a member of it.
- Grant the developer role the following rights to the second bucket created above.
   * create object
   * delete object
   * write to object
   * read object
 
  
## AWS CLI ##
Some things cannot be done in the AWS console, like scripting etc. Provide examples of AWS CLI (in a bash/zsh script) that can do the following:
- Show the contents of the hypothetical s3 bucket `Important Data/logs`
- Change the name of an IAM user
- Add the caller's IP address to a hypothetical security group `sg_3452925`
- Instantiate a new policy and attach it to the hypothetical role `developer_level2`

## Terraform ##
We use Terraform to manage infrastructure within our AWS accounts

Please create a Terraform (written in HCL) configuration to create and maintain the following resources:
- A t2.micro EC2 instance, named `workbench1`, based on an amazon machine image.
- A RDS Cluster with 2 nodes, each in different availability zone, with a max number of simultaneous connections equal to 16,000 connections.
- A pair of buckets, one pubic, one private with access to one external account with the account id: `001234567890`
- An IAM group containing 3 IAM users: `vera`, `chuck` and `dave`

# Software Development #
While we work on infrastructure, we do actually write code.  You need coding skills, both in writing code and working with various engineers throughout the company to help solve
problems and identify new requirements. Take some time to explain your development process as you demonstate your coding prowess. 

## Python ##
We use python heavily in our systems and infrastructure.  It's important to us that you demonstrate your software development skills, and python is an appropriate vehicle for that.
Write a simple AWS Lambda function in Python that reads data from an S3 bucket, processes it, and saves the results back to S3. Explain how you would structure the code and handle
errors.   If you don't know python, go ahead and use a language you are comfortable with; however keep in mind that you'll need to pick up python quickly if you accept a position 
with our team.

# ML Operations #
Our team is responsible for, among other things, developing and maintaine our ML Operations pipelines.  We use Sagemaker, and knowledge of the AWS Sagemaker suite is very helpful.
## SageMaker ML Ops ##
How would you operationalize a machine learning model on AWS SageMaker? Explain an end-to-end workflow from training to deployment, touching on model packaging, registration,
endpoints, and monitoring. Provide a code sample for deploying a model.

You have a machine learning model that needs to be containerized and deployed on SageMaker. Demonstrate how to dockerize the model and push it to ECR to prepare for deployment.

How would you monitor and retrain models deployed on SageMaker? Discuss using CloudWatch metrics, processing batch inference data, and automating retraining workflows. Provide sample 
code for implementing one of these.

# Final (important) notes... #
When you submit your exercise be sure to submit the following...
- Organize your code, each exercise in a different sub-directory
- In each subdirectory, include a markdown file describing each document/script, what it does, and how to use it.
- Include a markdown file at the top level that explains why you chose to not submit an answer to any item, a reason why it's not solvable (it's not supported by this method, etc).
- Everything you reference in your script, template, etc. should be included in this directory structure.  If the file is exceptionally large (like a model), provide the URL in the markdown file for that exercise so that we may fetch it during our review.
- Zip up your directory and submit it.

We don't need perfection, sharing why you might have run into a wall goes far in demonstrating to
us how you handle any roadblocks and how you might communicate to the team the situation when you seek assistance.


