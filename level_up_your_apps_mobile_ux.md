###Level Up Your Apps - Mobile UX

Optimize building your apps around the lazy, arrogant user that will use your app.

Think about how a hand is not opaque.  When things need to happen on screen and you need to see what is happening, make sure the action navigation is at the bottom.  Top navigation should be used for things when you no longer care about what is happening on the screen any longer.

Do one thing and do one thing well. - Multiple features, ONE PURPOSE

Make it easy to leave, make it even easier to return.

Google: "Our goal is to have our users leave our website as quickly as possible."

Being a great app means being great with other apps

Your app should provide functionality to other apps

If other apps provide functionality, use it

Navigation: Where am I?  What can I do here?  How did I get here?  Where can I go next?

Graphic Design:  "layout and typography are crisp and meaningful"

Font weights have meaning

When are things obvious?  When it's obvious to you, it probably isn't obvious to others.  You spend a lot more time looking at things than others do.

You will find most usability problems by just having 10 people use the app.  ~80% will be found by these 10 people.

Text -> Colors -> Icons  Order of design, differentiate text first, then colors, then add icons.

Moqups - online diagramming/mockup tool

Ideas from people of what should be in a conference app:

     share contact info using qr code
     my schedule
     whats happening now
     whats next
     notifications
     map of conference
     filters on topics you are interested in
     updated/change your personal schedule
     journal from conference or note taking ability (sharing as well)
     full conference search - conferences, sessions, speakers
     speaker bio
     push notifications of changes     

Users never care about how hard your app was to code, they just want how easy it is.

You should design your screens before you ever design your api endpoints.  You should always try to make only one api call per screen (or less).  Mobile latency is a problem, so make as few http calls as possible.

http://lab.to/oscon2013apk

mobile users hate being surprised

dialog boxes suck (same goes for modals) - don't take the user out of what they are doing

be fast, or if you can't be fast, pretend to be fast

be responsive - not RWD, but responsive in the terms of user input.  Lag equals death.

Instagram uploads pictures on android while you are writing about the picture so it appears that the upload is very quick.

google: "secrets to lightening fast mobile design"

never drop data - save state and restore it when a user comes back - app could crash at any time, so account for it.

lots of differing hardware, so make sure you account for different network connections, screen sizes, cpu/memory, etc.

minimize your views.  Views are expensive, and they should not be more than five levels deep.  Simplify things and refactor them to make it easy.

think about your first launch, make sure they can do what you want right away.

think about the mobile ecosystem, it's more than your app, so make it integrate with the other apps on your phone.

where am i? what can I do? what else can I do?  - think about these things for every app.

style your app, never port it from another platform, never make a generic app that for all platforms. looks bad on all of them then.

