# Loop for iOS

### Spike calibration guide: [Spike calibration](SPIKE_CALIBRATION.md), https://cyoung1024.github.io/spike-guide/calibration/

```diff
- Do not use this branch with rechargeable transmitters for Dexcom & Spike
- Always have alarms enabled for both lows and highs (also fast drop & fast rise)
- Read and follow the Spike calibration guide for every calibration
- Disable automatic boluses until you are able to get a good calibration
- Calibrate properly and often check the values reported by Spike against values from a glucose meter
```
If you are using Dexcom rechargeable transmitters please **use Spike in follower mode, with the Dexcom app as primary collector of data**.
This is because recently there have been cases of rechargeable transmitters providing inaccurate data. The Dexcom app has safety mechanisms built in, while Spike will report any data it reads from the sensor.

**What are the problems with rechargeable transmitters?**
- Multiple users reported noisy data.
- **If the transmitter's battery nearly runs out it will read HIGH**. It is extremely important to use the Dexcom app and Spike in follower mode to avoid this issue. If you're using Spike directly with the rechargeable transmitter, **Loop will deliver large boluses due to the erroneously reported increase in levels**.

# You are on branch spike-autobolus
This branch is a merge of https://github.com/LoopKit/Loop/tree/automatic-bolus and https://github.com/cyoung1024/Loop/tree/dev-spike.

Last updated on May 27, 2020

Last commit merged from automatic-bolus: https://github.com/LoopKit/Loop/commit/5fa561e2e74feca74f8115a2852ea3926ab27dcd

Last commit merged from dev-spike: https://github.com/cyoung1024/Loop/commit/79435954af008d1e3ae71304868be39016f9ef61

![App Icon](/Loop/DefaultAssets.xcassets/AppIcon.appiconset/Icon-Small-40%402x.png?raw=true)

[![Build Status](https://travis-ci.org/LoopKit/Loop.svg?branch=master)](https://travis-ci.org/LoopKit/Loop)
[![Join the chat at https://loop.zulipchat.com](https://img.shields.io/badge/zulip-join_chat-brightgreen.svg)](https://loop.zulipchat.com)

Loop is an app template for building an automated insulin delivery system. It is a stone resting on the boulders of work done by many others.

Loop is built on top of [LoopKit](https://github.com/LoopKit/LoopKit). LoopKit is a set of frameworks that provide data storage, retrieval, and calculation, as well as boilerplate view controllers used in Loop.

Please understand that this project:
- Is highly experimental
- Is not approved for therapy

<a href="/Documentation/Screenshots/Phone%20Graphs.png"><img src="/Documentation/Screenshots/Phone%20Graphs.png?raw=true" alt="Screenshot of status screen" width="170"></a>
<a href="/Documentation/Screenshots/Phone%20Bolus.png"><img src="/Documentation/Screenshots/Phone%20Bolus.png?raw=true" alt="Screenshot of bolus screen" width="170"></a>
<a href="/Documentation/Screenshots/Phone%20Notification%20Battery.png"><img src="/Documentation/Screenshots/Phone%20Notification%20Battery.png?raw=true" alt="Screenshot of battery change notification" width="170"></a>
<a href="/Documentation/Screenshots/Phone%20Notification%20Loop%20Failure.png"><img src="/Documentation/Screenshots/Phone%20Notification%20Loop%20Failure.png?raw=true" alt="Screenshot of loop failure notification" width="170"></a>
<a href="/Documentation/Screenshots/Phone%20Notification%20Bolus%20Failure.png"><img src="/Documentation/Screenshots/Phone%20Notification%20Bolus%20Failure.png?raw=true" alt="Screenshot of bolus failure notification" width="170"></a>

<a href="/Documentation/Screenshots/Watch%20Complication.png"><img src="/Documentation/Screenshots/Watch%20Complication.png?raw=true" alt="Screenshot of glucose complication on Apple Watch" width="141"></a>
<a href="/Documentation/Screenshots/Watch%20Carb%20Entry.png"><img src="/Documentation/Screenshots/Watch%20Carb%20Entry.png?raw=true" alt="Screenshot of carb entry on Apple Watch" width="141"></a>
<a href="/Documentation/Screenshots/Watch%20Bolus.png"><img src="/Documentation/Screenshots/Watch%20Bolus.png?raw=true" alt="Screenshot of bolus entry on Apple Watch" width="141"></a>
<a href="/Documentation/Screenshots/Watch%20Menu.png"><img src="/Documentation/Screenshots/Watch%20Menu.png?raw=true" alt="Screenshot of the app menu on Apple Watch" width="141"></a>
<a href="/Documentation/Screenshots/Watch%20Notification%20Reservoir.png"><img src="/Documentation/Screenshots/Watch%20Notification%20Reservoir.png?raw=true" alt="Screenshot of bolus failure notification on Apple Watch" width="141"></a>
<a href="/Documentation/Screenshots/Watch%20Notification%20Bolus%20Failure.png"><img src="/Documentation/Screenshots/Watch%20Notification%20Bolus%20Failure.png?raw=true" alt="Screenshot of bolus failure notification on Apple Watch" width="141"></a>

# Documentation

Please visit the [Loop Docs](https://loopkit.github.io/loopdocs/) for installation, algorithm, and other details.

For FAQs and other tips, refer to the [Wiki](https://github.com/LoopKit/Loop/wiki)

(Note: there is also a tab for the Wiki at the top of this page)

# License and Code of Conduct

Please read the [LICENSE](/LICENSE.md) and [CODE_OF_CONDUCT](/CODE_OF_CONDUCT.md)
