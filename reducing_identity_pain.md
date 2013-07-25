###Reducing Identity Pain

Tim Bray - Google - @timbray - tbray.org

Passport.js and Drywall.js are a couple of node.js user systems.

Usercake is another php one.

He says the user experience in both of the node.js ones are pretty good.

omniauth is one he says is not particularly damaging…

but don't use any of the above services he mentioned.

password managers are pretty good services - they are just too complicated for normal end users

>the harder you make the password requirements, the worse you make the internet.  "stop peeing in the pool."

[buyaccs.com](buyaccs.com) - you can go here and buy stolen accounts

people are more and more willing to use the login with facebook or twitter or google login options.

[favcolor.net](favcolor.net) - example page - [accountchooser.com](accountchooser.com) 

one click sign-in or two-click sign-up

[poetica.com](poetica.com) - looks at the email address and uses mx record for the domain and then asks you to sign in with that idp.

idp = identity provider

google is betting on oauth2 & openID as the identity protocols

use https for everything, then you wont accidentally not use it for an important thing

[tbray.org/ongoing/When/201x/2013/04/04/ID-Tokens](tbray.org/ongoing/When/201x/2013/04/04/ID-Tokens)

fancy.com - shows a simple example of using google+ sign-in page

cross-client identity: unicorns & rainbows - allowing users who are logged in on one device to have an easy ability to get in on other devices. - its a little extra work, but work that you should be doing.

[developers.google.com/accounts/cookbook](developers.google.com/accounts/cookbook)

**last thoughts:**

- get out of the password business and get into the federated identity ballgame.  
	- please be kind to your users, 
	- don't make your users type passwords, 
		- especially on mobile devices, 
	- and don't get crazy with crypto passwords.
- use libraries, don't try to do crypto by yourself
- get out of the business, you are decreasing the quality of the internet, and decreasing the quality of your applications.