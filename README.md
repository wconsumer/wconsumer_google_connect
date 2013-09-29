Connect with Google (wconsumer)
========================

Implements "Connect with Google" feature allowing user to sign in or sign up with his Google account. 

User flow is as follows:

1.  User clicks Connect with Google link in login form.
2.  Module authenticates user with Google and retrieves his Google account data.
3.  If there is a user registered in Drupal having same Google url ('public_url' field of Google /user response) then user is logged in with this account.
4.  If there is no such account then try to register user with his Google login and email.
5.  If registration fails (login or email already taken, etc) then redirect user to the register page and allow him to manually register a new account.

