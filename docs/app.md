# Minimal Phone

This app strips your phone of its addictive and unproductive aspects. It distills the device down into essential functions that is important to everyday life. Such as internet banking, e-wallets, 2FA authenticators, mandatory university apps, etc. 

This app exists because of how toxic smartphones can sometimes be to our well-being. Yet, dumbphones can be expensive and downright too restrictive which makes it impractical for everyday use.

# Mechanism

Minimal Phone limits the apps that can be installed on your phone. It also deletes the browser, since most social media apps have a web version. In the future a limited browser may be included in the suite to provide essential support (e.g. for web based OAuth authentication), but it isn't available yet because of current development constraints.

Because each country usually has its own ecosystem of apps (e.g. different banks, e-wallets, universities), the list of allowed apps is governed by the community. For edge cases, you may enable the experimental LLM-as-a-judge feature (coming soon) (more important for the novel limited web browser feature).

# Flow

The app starts by opening the Device Policy Manager (DPM) provisioning screen. 

On Android, there are only two ways to provision a DPM: through a factory reset or through an ADB command.

Traditionally, commands to ADB could only be issued from a connected computer. With the advent of wireless debugging, however, this is no longer the case. Minimal Phone uses Shizuku, which leverages wireless debugging to issue the required provisioning commands without the need for a separate computer.

But Android refuses to set an app as a DPM when there are accounts connected in your phone. So you need to log out of all accounts before you're able to perform this. Be careful of locking yourself out, remember the passwords and make sure you have a way to perform the 2FA, if you have them.

# Deliberate Friction

## Delay-based Friction

## External Approval

## AI-based Approval

> *This app serves as a blank slate for future Productive-Social Phone concept I have in mind, but let's leave that for later.*
> *This app aims to avoid being to rigid and hard to configure like Plucky, so it's more easily usable.*
