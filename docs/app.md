# Minimal Phone

Minimal Phone turns your android phone into a minimal phone, stripping it from its addictive nature.
It turns your phone into something you intentionally pull when you need something, not whenever
impulses pull you in.

There are several ways Minimal Phone tries to do this, it does so by:

- Limiting the apps that can exist in your phone.
- Limiting browser capability.
- Replacing what has been restricted with something better.

Minimal Phone achieve this by utilizing Android Device Policy. 

Android Device Policy is a feature that corporations use to manage company-issued phones,
and limit their functionality to only what is directly aligned with their missions.

Although in this case there is no corporation at all, Minimal Phone utilizes the deep restriction 
capability of Android Device Policy to turn your smartphone into a minimal phone. Without you
needing to take any money out of your pocket to buy a feature phone. 

Additionally, Minimal Phone allows you to use important apps that dumb feature phones doesn't have
the ability to support. Such as 2FA Authenticators, Mobile Banking, E-Wallets, University  Apps, etc.

## Mechanism of Lockdown

Minimal Phone keeps a list of allowed app.

Initially you set a select few of allowed apps before activating lock down, this list is kept
flexible at first because the unknown numbers of apps the user might legitimately use in their
daily life.

After the phone is locked down, no further changes are applied as easily.

Minimal Phone enforces delay before any configuration changes are applied to the settings. This
eliminates many impulse-based changes the user may try to do. But there are genuine practical 
needs that users may sometimes have that they need to be done quickly.

So to accomodate those quick just-in-time needs, Minimal Phone allows your friend to approve
your changes to be in effect immediately. Furthermore, Minimal Phone offers an experimental
LLM-as-a-Judge feature that can cover worst case scenario like inaccessible friend contact.

## Browser Restriction

Browsers have always been a tricky space that need to be tackled smartly. Removing browsers
altogether risks making a considerable amount of apps unusable. Because they may require browser
based login mechanism.

There are a few control mechanism that can be used:

 - Restriction through DNS
 - Restriction through Forced Install Extension (only available on Microsoft Edge)

Experiments need to be done to prove which method is the best.

DNS-based restriction may not work well in environments which require the user to use a WiFi's
assigned DNS in order to access certain services. This happen to me personally on college.
