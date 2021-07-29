## Hola amiguitos

This is my attempt to fix up and add a little crDroid customization flavor back into the sdm845 kernel tree for OnePlus 6 & 6T (enchilada & fajita).

Rebased on the official lineage-18.1 branch from LineageOS as of October 2021, with some extra goodies added in like clang 12 & 13 support, multiple vibration type support, wireguard support, and battery-idle-mode-enabled charging switches.

Also added AnierinB's stack of tweaks from the Evolution-X version of the oneplus_sdm845 kernel, since they know better than me what things need some love.

I also reworked the DC Dimming (among other things) commit substantially, and everything seems to work. Like, shockingly well. Then I did it AGAIN when the OOS 11.0 source came out, and it's STILL working. I am more surprised than anybody, I'll be the first to admit. No more relying on bizarro-world "main_display" symlinks that make the SDM845 kernel different than all the other, newer OnePlus devices, making it difficult to implement features like DC dimming, etc. in the device tree... which was important up until just a little bit ago when AnierinB made a universal DeviceExtras package. Welp.
Still helps.

If anyone is still reading, hi. You're pretty cool. There has been a lot of work on this, and most of it will never be visible, but at least you know I spent many hours of blood, sweat, and hair-pulling trying to test & fix things; and then most of that work was repeatedly rendered moot, but some of it at least has been getting picked up & cleaned up by smarter people than me and hopefully everyone will get to benefit from it.

Not TOO shabby for someone who doesn't actually know any c/c++/java. :D
