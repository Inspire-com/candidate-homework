Inspire QA Engineer Automated Testing Exercise

We would like you to do the following exercise to show us how you might use automated testing to run regression tests on our flagship site, https://www.inspire.com.  

We would like you to post a journal entry that only you can read.  In order to get familiar with our site, please make yourself a username and password and click around a bit.  Please note that you are going to need to give us the credentials for this account as part of your test script.

You may use the automated testing platform of your choice.  This is not a timed test but it should not take you more than 30 minutes to complete.

Step 1.  Create a username/password using an email address on inspire.com.  For the purpose of this test, please use an email login instead of social login. This part of the test is manual and you do not need to automate it.  You will use these credentials in your automated test.

Step 2. Email your inspire contact your account credentials.  We will need to enable your account to bypass captcha.

Step 3. Create a short test script to do the following.

```Log into https://www.inspire.com
Click on “Start a Journal Entry”
Fill out the “title” input field.
Fill out the “Body” input field

Do not select any communities.  (Since this is a test, we just want the journal entry visible to you)

For “Share with” select “inspire friends” (With a new account, you won’t have friends yet so this will post just to you.)

Click Post

Verify that your post shows up at the top of the lists of posts in your journal by looking for the text you used to input. 
```
Deliverables:

  1. Which testing framework did you choose and why?
  2. Setup instructions for how to use your testing framework.  You can point us to specific resources, but please assume we have never used it before when you introduce us to it.
  3. Your actual test suite zipped up in a format we can run.
