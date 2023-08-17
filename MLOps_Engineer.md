#ML Ops Engineer

## Show us what you can do ##

_If any part of this exercise is unclear, please don't hesitate to ask us questions. If you feel it is taking more time to accomplish than you have to commit, please let us know that as well. Our goal is not to waste anyone's time, but to have a simple set of exercises you can use to demonstrate your skills. These are basic functions that you should feel confident in demonstrating and performing on a daily basis._

### Infrastructure as Code ###

Much of our work is managing the infrastructure on which we manage our systems.  One of our mottos is *Infrastructure as Code*, and to this end, we heavily use AWS CloudFormation, Terraform, CDK and CLI to manage our systems _including ML Ops_.   

_We prefer CloudFormation for this submission, However if you cannot write this in CloudFormation, you have other options..._0

1. Implement using TerraForm
2. Write a bash script using AWS CLI
3. Write a python module that uses CDK or BOTO3
4. Record yourself performing these functions via the AWS Console._

Please create a CloudFormation document that can be applied to AWS and configures the following services:
1) Instantiate SageMaker Domain
2) Create a SageMaker Notebook instance
3) Instantiate a basic SageMaker Pipeline, your pipeline should do the following:
   a) train a model
   b) deploy the model to the registry
   c) deploy your model

### Finally ###

Document your submission!   Talk about stumbling blocks, clarify your decisions for us, show us what you do so that the next engineer who might look at your code in the future and need to maintain it, will be able to carry the baton.

We look forward to your submisson and discussing it with you!
