Inspire QA Engineer Automated Testing Exercise

We would like you to do the following exercise to show us how you might use automated testing to run regression tests on our flagship site, https://www.inspire.com.  

We would like you to post a journal entry that only you can read.  In order to get familiar with our site, please make yourself a username and password and click around a bit.  Please note that you are going to need to give us the credentials for this account as part of your test script.

You may use the automated testing platform of your choice.  This is not a timed test but it should not take you more than 30 minutes to complete.

Step 1.  Create a username/password using an email address on inspire.com.  For the purpose of this test, please use an email login instead of social login. This part of the test is manual and you do not need to automate it.  You will use these credentials in your automated test.

Step 2.  Create at least two posts on the site so you can get familiar with the site and then email the account credentials you created for this test to your Inspire contact.  We will need to enable your account to bypass captcha so you can finish your test.  You can create posts that are friends only so they will not be visible to anyone but you.

Step 3. Create a short test script to do the following.

```Log into https://www.inspire.com
Click on “Start A Post (Discussion Or Journal)”
Verify the overlay pops up.
Click on "Post an Entry in my Journal"
Under "Post in these communities:" chose "Select None"
Create a title in the “Title” input field.
Write some content in the “Body” textarea.
Under the "Share With" heading, select the "Inspire friends" racdio button. (With a new account, you won’t have friends yet so this will post just to you.)
Click Post

Verify that your post shows up at the top of the lists of posts in your journal by looking for the text you used to input. 
```
Deliverables:

  1. A brief paragraph explaining which testing framework you chose and why?
  2. Your test scripts.  You can email them zipped up or give us a github repo to check out.
  3. Instructions for us on how we can run your test scripts.
