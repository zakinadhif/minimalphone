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

## Modes of Activation

Minimal Phone has two modes:

 - Enforcing (All frictions active, all lists enforced)
 - Permissive 
 - Disabled

## Teardown Mechanism

When the Enforcing mode is activated, your list of allowed apps, and websites are enforced.
This mode can't be easily deactivated, it must go through the friction mechanism first.

## Friction mechanism

 - Friction by delay
 - Friction by external approval

Friction by external approval includes two possible party:

 - Another person (your friend, family, strangers)
 - AI agent

## AI-agent based External Approval for Application List Request

This method trades friction-robustness by convenience, meaning you don't have to call your friend to approve your changes in time of need, but you give in to the possibility that the AI may incorrectly classify your request.

## AI-agent based External Approval for Browsing Request

This method is much more needed than the App List Request variant because the vastness of the internet, in the future this may become the default.

The friction are applied by an AI agent sitting in a Browser extension, stopping any response before it is parsed by the browser and examining it from any suspicious content. If such are detected, the domain will be blacklisted and no further examination may be redo except by explicit request.
