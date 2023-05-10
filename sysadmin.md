
If any part of this exercise is unclear, please don't hesitate to ask us questions. If you feel it is taking more time to accomplish than you have to commit, please let us know that as well. Our goal is not to waste anyone's time, but to have a simple set of exercises you can use to demonstrate your skills.

### CloudFormation ###

Much of our work is managing the infrastructure on which we manage our systems.  One of our mottos is *Infrastructure as Code*, and to this end, we heavily use AWS CloudFormation.

Please create a CloudFormation document that can be applied to AWS and configures the following structure.
1) Instantiates a pair of s3 buckets.
2) Create and apply a pair of policies, one that sets one of the buckets to be public, the second to be private.
3) Create a `developer` role and make `vera` a member of it.
4) Grant the `developer` role the following rights to the second bucket created above.
  - create object
  - delete object
  - write to object
  - read object

### AWS CLI ### 

Some things cannot be done in the AWS console, like scripting etc.  Provide examples of AWS CLI (in a bash/zsh script) that can do the following.

1) Show the contents of the hypothetical s3 bucket `Important Data/logs`
2) Change the name of an IAM user
3) Add the callers IP address to a hypothetical security group `sg_3452925`
4) Instantiate a new policy and attach it to the hypothetical role `developer_level2`

### Terraform ###

We use Terraform to manage AWS accounts

Please create a Terraform (written in HCL) configuration to create and maintain the following resources:
1) A `t2.micro` EC2 instance, named 'workbench1', based on an amazon machine image.
2) A RDS Cluster with 2 nodes, each in different availability zone, with a max number of simutaneous connections equal to 16,000 connections.
3) A pair of buckets, one pubic, one private with access to one external account with the account id: `001234567890`
4) An IAM group containing 3 IAM users: `vera`, `chuck` and `dave`

The output of this exercise should be a zip file containing a set of files as well as a markdown file describing each document/script, what it does, and if you're unable to complete an item, simply a reason why it's not solvable (`it's not supported by this method`, etc). 
