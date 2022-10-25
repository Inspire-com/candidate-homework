# Inspire QA Engineer Automated Testing Exercise
## Part 1
We would like you to do the following exercise to show us how you might use automated testing to run regression tests on our flagship site, https://www.inspire.com.  

We would like you to post a journal entry that only you can read.  In order to get familiar with our site, please make yourself a username and password and click around a bit.  Please note that you are going to need to give us the credentials for this account as part of your test script.

Please use Python and Selenium to complete the rest of this exercise, but feel free to use a BDD-based component such as Behave as well. This is not a timed test but it should not take you more than an hour or two to comprehensively complete. Keep in mind we will be looking not only at the content of the exercise submission, but its structure, thoroughness and modularity.

### Step 1.
Create a username/password using an email address on inspire.com, and chose a user name like QA_candidate_1.  For the purpose of this test, please use an email login instead of social login. This part of the test is manual and you do not need to automate it.  You will use these credentials in your automated test. In addition, you will need to join a least one community.

### Step 2.
Create at least two posts on the site so you can get familiar with the site and then email the account credentials you created for this test to your Inspire contact to help us evaluate your submission. You can create posts that are friends only so they will not be visible to anyone but you.

### Step 3.
Create a short test script to do the following.

```Log into https://www.inspire.com
Click on “Create Post”
Verify the overlay pops up.
Click on the "Choose Community" and choose a community you joined in Step 1.
Click on the "Choose Topic" and choose any topic.
Create a title in the title input field.
Write some content in the body textarea.
Click the "Privacy" dropdown menu and choose the "Inspire Friends" option
Click Post
Verify that your post shows up at the top of the lists of posts in your account by looking for the text you used to input. 
```
Deliverables:

  1. A brief paragraph explaining the methodology in your submission (how classes are organized, BDD component choice, etc)
  2. Your test scripts.  You can email them zipped up or give us a github repo to check out.
  3. Instructions for us on how we can run your test scripts.

Note that your submission must successfully run strictly on your instructions, so please write them with care
