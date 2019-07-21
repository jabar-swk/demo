This is an example of a typical website that implements SimpleLogin. 

Upon successful login, you will see the information that the website receives 
when you sign in with SimpleLogin.

This website also features Facebook login for comparison.

This is a front-end only web-app, none of your data is saved or used 🙂, even for analytics purpose. 

This project depends on:
- Bootstrap 4
- VueJS

This website can be served via any static server, for example with `http.server` python module:

> python3 -m http.server

It works immediately with SimpleLogin as SimpleLogin whitelists localhost to facilitate development.

For Facebook, unfortunately you would need to:

1. create a Facebook app on https://developers.facebook.com
2. replace the facebook app id used in `index.html` by this appId 

```<script async defer crossorigin="anonymous"
    src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v3.3&appId=410139219846977&autoLogAppEvents=1"></script>```

3. run a https server, add this domain to facebook.  

These steps are required because Facebook SDK does not allow http://localhost by default.

