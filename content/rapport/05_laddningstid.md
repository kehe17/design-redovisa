---
---
Load Time
=========================

In this article I will document and analyze load times of different web sites. I gathered data using Google's PageSpeed Insights as well as devtools in Google Chrome.  I opted to use the same sites as in the previous article about color schemes.

Paradox Plaza
-----------------------

[FIGURE src=image/colors01.png?w=742 caption="[Paradox Plaza](https://forum.paradoxplaza.com 'Paradox Plaza')"]

Paradox plaza received a PageSpeed score of only 45, in the devtools test it came in at an average load time of 2.35 seconds. With a 4.9MB payload, it's not surprising that it was the worst performer of the three sites. According to PageSpeed, the biggest improvement to load time would come from serving images in next-gen formats.


GitHub
-----------------------

[FIGURE src=image/colors02.png?w=742 caption="[GitHub](https://github.com 'GitHub')"]

GitHub's PageSpeed score was a bit more flattering at 64, while the average load time in the devtools test was 0.73 seconds. Despite sporting a 4.2MB payload it loaded practically as quickly as the much lighter Discord. Again PageSpeed suggests that the biggest improvement to load time would come from serving images in next-gen formats.


Discord
-----------------------

[FIGURE src=image/colors03.png?w=742 caption="[Discord](https://discordapp.com 'Discord')"]

Discord received the best score from PageSpeed of 72 and came in with the lowest average loading time in the devtools test at 0.69 seconds. With only a 1MB payload I expected this to perform the best. Main improvement to load time here would be to minimize main-thread work and reduce JavaScript execution time according to PageSpeed.


Other
-----------------------

There is definitely a trend to be observed in the results, with the largest improvements being found in optimizing images. Large savings are estimated from properly sizing images, serving images in next-gen formats, efficiently encoding images (aren't these two really the same?) and avoiding enormous network payloads (which, I suspect, is directly caused by ineffecient images). In terms of ranking the sites, I think it's safe to say Discord wins. GitHub and Paradox Plaza both have unnecessarily large payloads, GitHub ranks second thanks to still loading in less than a second and Paradox winds up last.

[Raw data](https://docs.google.com/spreadsheets/d/1AZWYISav3dtwMAW9_PKmOIMXacBdEmVes0VY1aVmBNU/edit#gid=0 'Google sheets')

Author: Kenneth Heimer
