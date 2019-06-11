---
layout: post
title: The 4.2 - IIIIII release is finally here!
image: https://raw.githubusercontent.com/BootleggersROM/ExtraStuff/pasta/blogstuff/bootleg_42_iiiiii.jpg
---

Hello everybody! Hope you're having a nice monday. After almost 2 months of a bit of work mixed with some difficulties, we can finally release our 4.2 release. Our musical codename is [**IIIIII**](https://www.youtube.com/watch?v=yeeK5aQSzRo) because it's the most accurate representation about this release went.
We got a bit of a chaotic month between some time constraints, some attempt to get a gerrit working, but then, we did a bit of work on the sources and we feel that it could go better but we can't delay this release anymore, so, here we are.
We have some small news about this release and some extra stuff we want to tell you so, fasten your seatbelt, here we go!

**A medium size release, but with some love in it**

This release includes some changes related to telephony (some cleanup made to support future devices in a better way, like violet, shoutout to merothh for doing this), some support for OnePlus fingerprint devices, some fixes from our part related to the screenshot editor app (credits to shagbag913 for telling us and for the potential fix) and some under the hood things. Feature wise, we added LS date styles, which was a pain to bring up due to the massive difference between the oreo and pie implementation. We did some ugly work but it's finally there. We have to thank DirtyUnicorns for implementing that thing back on oreo, and it was missing on pie. But wait, there's more. We not just brought that back, we added some new designs with some gradients because, those lockscreen clocks needs some gradient companion. Also, we added android q clock, which is nice, but currently it has some issues related to refreshing the accent, so a systemui restart might be required? Credits to Potato, Descendant and AOSiP for their work on that gorgeous text clock. 
Most of our changes are pretty under-the-hood changes to add more support to new devices (we even saw bootleg run on a Pixel 3A, which is interesting, and also, massive shoutout to DU team for their bonito/sargo sources, those made it possible to boot, and last but not least, shoutout to stebomurkn420 to experiment with those sources).
There might be some issues for Indian users and maybe in other country users when they try to open developer option, it is due to translations, so feel free to check if your translations are fine on our [crowdin](https://crowdin.com/project/bootleggers-rom) and help us correct some of those translations, or even, translate the new features and stuff.

As we did previously on 4.0 to 4.1, there's the changelog between 4.1 and 4.2
```
* Added translations
* Fixed emergency icon tinting, credits to PE
* Rebased telephony repos
* Lockscreen date styles
* Shishu Themes now have LIT instead of LTE
* Added Q clock with extra changes for date and owner
* Aggresive Battery
* Custom fingerprint icons for OP devices 
* Fixed Markup building for all devices
* Added Q seekbar with a small ui change
* Added improvements for 3 finger screenshot
* Re-introduced Woodman due to devices bootlooping
* One Hand UI
* Pixel Navbar animation
* Some extra undocumented kanging for legal reasons
* Added some new QS styles
* Fixes and improvements
* Launcher3 now has the window to icon animations, and also, fixed dark google feed
* Revert: Revert: [DO NOT MERGE] Partial Revert of john woodman
```

As always thanks to our maintainers for giving info, some ideas, and a extremely testing of all the new things to come. And also, a massive shoutout to our internal tester team, who was giving reports of our sources working fine for a daily usage. Now, we want to share something really interesting with you

**A font pack of your own?**
_Editor's note: this is added because we thought it's an incredible idea and we have to thank the Carbon Team for creating this tool. If you have issues with it, feel free to report to them, not to us._

Sometimes you're on a ROM that got the incredible feature that's FontService, the thing that it got a font pack, and you like that feature, but suddenly, your childhood memories of doing digital drawings and writing in comic sans comes back to your memory. You shed a tear, you feel nostalgia for the almighty, sometimes unfarirly hated font and you want it on your good lookin' Android device.
If it's that's your case, please **get some help.**
Now, in the case that you know what a ttf/otf file is, and you got your favorite font in that format, and you want to do your own pack with custom fonts, well.. carbon got a solution for you! Introducing: the CarbonROM font package generator!
It's a website where you can put your favorite fonts and it will do an apk ready to be used anywhere! No matter which rom you're going to. If they have FontService, then, the package will work. 
You can create [your own font pack right now](https://fonts.carbonrom.org) or, if you want to help Carbon in the matter of costs to keep this incredible tool up, feel free to [donate to them](https://www.paypal.com/donate/?token=_noJxcxnGA0SY-CkQxyXr7kypvPX8--D3znNiVIYHvNOWbcsOjnVa4KMiG2jih_JBl5eL0&country.x=US&locale.x=US)! They deserve it a lot.

**Wrapping things up, and also, speaking of donations...**

Hope you enjoy this new release, and also, have fun with that awesome tool to make your own font packs! We want to make you feel like 家 and something like that tool actually does a lot. So, as always, we thank to all the ROM devs that are working an incredible job in making custom roms something _breathtaking_. Do you have any questions, love for the update or hype about it? Feel free to share it on our [Telegram group](https://t.me/keepthebootleg) or even talk about music or whatever on our [OT group](https://t.me/keeptheshitposting). Mama would say that the releases will be up when the maintainers can do it, so please, don't ask for ETAs or spam the poor maintainers about it. They're doing an incredible work in giving you the best experience.

About the donations part... We decided to finally open a donation section, so, if you appreciate the shishu themes, or the ROM overall (even though, we're actually not doing a lot of work in the part of coding, but we try), feel free to donate to the [Lead dev](https://bootleggersrom.github.io/donate). With your support and donations we can go further. From paying some english lessons, or pay a server to have a better infrastructure or even have a gerrit to work better and faster till stop relying on Google Cloud trials and purchase a building PC... doesn't matter. The thing is, if you want to support us, we'll appreciate it a lot. We have a lot of plans in the future, so stay tuned! 

Hope this release makes your monday/tuesday a bit better, and as always, Keep the bootleg.
