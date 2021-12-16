
If any part of this exercise is unclear, please don't hesitate to ask us questions. If you feel it is taking more time to accomplish than you have to commit, please let us know that as well. Our goal is not to waste anyone's time, but to have a simple set of exercises you can use to demonstrate your skills.

### CloudFormation ###

Much of our work is managing the infrastructure on which we manage our systems.  One of our mottos is *Infrastructure as Code*, and to this end, we heavily use AWS CloutFormation.

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

Some things cannot be done in the AWS console, like scripting etc.  Provide examples of AWS CLI (in bash script if necessary) that can do the following.

1) Show the contents of the hypothetical s3 bucket bucket `Important Data/logs`
2) Change the name of an IAM user
3) Add the callers IP address to a hypothetical security group `sg_3452925`
4) Instantiate a new policy and attach it to the hypothetical role `developer_level2`

### Ansible ###

We use Ansible to keep our linux systems up to date and configured according to our standards.

Please create an Ansible playbook that can be run against an Ubuntu 20.04 Linux server and would do the following:
1) Install all updates
2) Create a new user account called “inspire”
3) Create a password for the “inspire” user, also set to “inspire”
4) Create a file in the "inspire" user's home folder called “inspire.txt” with the text “Inspire is awesome” inside the file.
5) Ensure that the apache web server is installed, is running, and starts up automatically if the system is rebooted.

The output of this exercise should be a single Ansible playbook. We will examine your playbook and test it against a fresh Ubuntu 20.04 linux virtual machine in EC2.
