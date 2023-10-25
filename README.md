# Playdate-LuaQRCode

This is a fork of
[speedata/luaqrcode](https://github.com/speedata/luaqrcode)
for the Panic Playdate included with the
[PlaydateSDK](https://play.date/dev/).

The base of the fork was [speedata/luaqrcode#2389b18](https://github.com/speedata/luaqrcode/tree/2389b18780cfc7653f72a3e225e4522b6ec4426d)
(2017-01-05) and Panic added a couple small changes
to enable cooperative multitasking via `coroutine.yield()`.
You can see those changes in [this commit](https://github.com/notpeter/playdate-luaqrcode/commit/ecfb836fe7718773c4c5aa2633511b69d228ad97)

This repo has three branches:
* [master](https://github.com/nopeter/playdate-luaqrcode/tree/master)
which tracks upstream master ([speedata/luaqrcode](https://github.com/speedata/luaqrcode/tree/master))
* [playdate_sdk](https://github.com/notpeter/playdate-luaqrcode/tree/playdate_sdk)
which tracks the current qrencode_panic_mod.lua shipped in the PlaydateSDK.
* [playdate_new](https://github.com/notpeter/playdate-luaqrcode/tree/playdate_new)
which includes changes from playdate_sdk branch and upstream master.

If you are seeing this readme, you are are looking at the playdate_new branch.

If you wish to inspect these files as included in the PlaydateSDK, see:
* `CoreLibs/3rdparty/qrencode_panic_mod.lua`
* `CoreLibs/qrcode.lua` (implements [`playdate.graphics.generateQRCode`](https://sdk.play.date/Inside%20Playdate.html#f-graphics.generateQRCode) wrapper)

## Legal

The qrcode library is licensed under the 3-clause BSD license (aka "new BSD")

This fork is unaffiliated with Panic Inc or Patrick Gundlach,
please do not contact them for support.

# Original readme:

See the homepage at http://speedata.github.io/luaqrcode/ for more information.

Special thanks to all contributors. Everything helps: bug reports, patches etc.

License: 3-clause BSD license<br>
Usability status: mature, used in production<br>
Maintenance status: maintained (bug fixes)<br>

Part of the [speedata Publisher](https://www.speedata.de/).
