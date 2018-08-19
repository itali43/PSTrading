![icon](https://github.com/itali43/PSTrading/blob/master/PSIcon.png "icon")     ![preview](https://github.com/itali43/PSTrading/blob/master/preview.png "preview")
# Application Story + Showcase:  Purple Swan Trading 
### Or how I built a Mobile GDAX Trading application and didn't publish it.

#### Long Ago in a Galaxy Far Far Away, there was a dream-- 
and that dream was to be able to trade on GDAX on a mobile phone.  And this dream was built-- shoe-horned into any free time I had between jobs --so that I could finally panic buy, panic sell and just generally make sound and farsighted financial decisions about my cryptocurrency hodlings from my mobile phone.  And after many long evenings-- success!  An App had been formed.  And it worked.  It even had some easter eggs and professional design input built in!  

So time to publish it right?

But alas, it was not to be.

Apple, in their infinite wisdom, decided that having financial institution's private keys in a third party app (even if that app was specifically designed to have no connection to any servers except said financial institutions!) was a no-go, see App Review Guideline 3.2.1(viii)*:
~~~
(viii) Apps used for financial trading, investing, or money management should come from 
the financial institution performing such services or must use a public API offered by 
the institution in compliance with its Terms & Conditions.
~~~
* <sub><sup>For More Light Reading, See Source: https://developer.apple.com/app-store/review/guidelines/#acceptable</sup></sub>

### ❤️ -> 💔

So, it seems my exciting new GDAX Trading Application will forever be only useful to me.  No public release to the App Store. But enough story, here's what it looked like:

Anyway, Enough Story.

# Trading Feature Summary

## Login
The Log in is actually one of the coolest parts of the feature set.  It's decentralized.  Nothing complicated, just that the login is specific to the device.  Purple Swan operates without it's own server (using only Fabric and the various exchange APIs for in/outgoing network traffic).  This was designed this was such that no one could touch your private keys except you.  The login, password and all of the three Private API keys (see credentials section) are stored on the digital keychain of your phone, for safe (and decentralized) keeping.

There's also a cool animation where the swan looks like it swims back to the left when you click the "< Trackers" button (trackers = price trackers).  It makes it look like it swims off the screen and back into the center of the Purple Swan Price Checker App.
  ![loginAnimation](https://github.com/itali43/PSTrading/blob/master/logout.gif "LogInAnimation")

And just in case you want to read the far too wordy explanation at the bottom: 
> > And Trade Mobily. PS Username/Password are for convenience security so you don't need to enter your API keys every time you trade. They are stored on your phone's keychain and are accessible only locally by your own Purple Swan App instance. Only server ever touched is GDAX, everything else is stored locally! If you forget your password/username, just make a new one and re-enter your API Keys. Happy trading, and of course...  To The Moon! 🚀


## Start Trading!
Once you log in / sign up you get to the main page.  Note the pleasant looking graph with multiple time horizons to peruse, the lock and key up top which is how you get to the credentials section, and the greyed out Execute button for no errant buy/sells upon first initiating the trading functionality.  

![startTrade](https://github.com/itali43/PSTrading/blob/master/startTrade.png "StartTrade")


## Buy
Note, once you press buy and change to a Limit Order, a limit price textfield appears, and an option to Kill all Limit Orders as well.  It asks to confirm, as all trading decisions on PSTrading request, and then can cancel your whole limit book.

![Buy Trading](https://github.com/itali43/PSTrading/blob/master/buyTrading.png "Buy Trade")


## Sell
Colors change and limit price textfield disappears too, as I clicked back to Market orders as well.

![sellTrade](https://github.com/itali43/PSTrading/blob/master/selltrade.png "Sell Trade")


## Credentials
Good news, I blacked out my API keys twice over, so that you can't use them for any nefarious purposes, hooray!  Basically you can generate these when logged into your GDAX account, and then type them into here.  Every time you leave the page your API keys are saved to the device's Keychain.  This keeps them secure on the device as well as completely localized-- but still allowing for easy use of the app (without having to enter them every login).

![creds](https://github.com/itali43/PSTrading/blob/master/cred.png "creds")


# Resolution:  Purple Swan LAMBOFolio

 After spending the after the App Store rejection day a bit sad, I decided to make something great to fill the feature hole I had in my production timeline, and two weeks later I posted the LAMBOFolio feature.  Far less serious than PSTrading, it makes Lamborghinis fall from the sky depending on how many bitcoin you tell it you have.  So just in case you wanted to splurge all of your crypto gains on Lambos, you know what it would look like.
 
 ## Raining Lambos (usefulness level: 💯)
 ![lambo](https://github.com/itali43/PSTrading/blob/master/rainingLambo.png "lambo")


I'd encourage you, dear reader, to check it out [here](http://swan.agrippa.tech)

## Conclusion
The skills and experience I gained building out Purple Swan Trading were worth the efforts, despite the anti-climactic, mothball ending 🧐, but I would highly suggest one reads the App Review guidelines with a fine-toothed comb before embarking on too long a journey. 
# 🌊🚢







