OGameTradeCalculator
====================

This script adds a trade calculator to the [OGame] interface. Allows you to save your favorite ratios, use percentages, export the results as an awesome ogame message, etc.

Installation
------------

  1. Install [Greasemonkey] \(for [Firefox]\) or an alternative, like [Scriptish] \(for [Firefox]\) or [Tampermonkey] \(for [Chrome]\).
  2. Click this [install link] and accept the installation.

Is this script tolerated?
-------------------------

Yes, this tool is [tolerated by OGame Origin], so you can use it in any server.

Languages
---------

The available interface languages are:
  - **English** (*default language*)
  - **Español** (*ogame.com.es, ogame.com.ar, mx.ogame.org*)
  - **Française** (*ogame.fr*)
  - **Italiano** (*ogame.it*)
  - **Nederlands** (*ogame.nl*)

You can send me more [translations].

A quick look at the calculator
------------------------------

![screenshot-calculator]

It allows you to calculate:

  - One output resource giving one input resource.
    *For example: 300 Metal = 100 Deuterium.*
  - One output resource giving two input resources.
    *For example: 300 Metal + 200 Crystal = 200 Deuterium.*
  - Two output resources giving one input resource and the splitting percentages.
    *For example: 600 Metal = 200 Crystal (50%) + 100 Deuterium (50%).*

Features:

  - You can write your custom ratios or pick one from the dropdown.
  - If the ratio you wrote is illegal the calculator alerts you.
  - It displays the total amount of resources which will be sent and received.
  - It displays the required amount of small/large cargo ship for shipping those resources.
  - Makes a colored message for sending the trade offer to other players.
  - You can especify the delivery planet or moon on the message.

Settings > Ratio list
--------------------------

![screenshot-ratio_list]

It allows you to modify the ratio dropdown of the calculator, for quick-picking the most used ratios instead of writing them manually.

Features:

  - Edit, add, delete and sort ratios.
  - Select the default ratio.
  - Edit the maximum and minimum ratios (used to check the legality of other ratios).

Settings > Default values
------------------------------

![screenshot-default_values]

The screen capture it's pretty selfexplanatory, this section allows you to pick the default values which are selected every time you open the calculator.

Options:

  - Select the default action (buy or sell).
  - Select the default output resources (metal, crystal, deuterium, metal+crystal...).
  - Automatically select the current planet or moon as delivery place.

Settings > Abbreviations and autocomplete keys
---------------------------------------------------

![screenshot-abbreviations]

Options:

  - Use abbreviations.
    *For example: Displays `3.5M` instead of `3,500,000`.*
  - Unabbreviate fields on mouse over.
    *For example: A field is displaying `500K` if you put the mouse over it, it will display `500,000`.*
  - Pick the abbreviation for millions and thousands.
    *For example: If you pick `KK` as abbreviation for millions, then `3,500,000` will be displayed as `3.5KK`.*
  - Pick the shortcut key for millions and thousands.
    *For example: If you pick `k` as shortcut for thousands then if you write `23kk` it will automatically change the field to `23,000,000`.*

Settings > Message template
--------------------------------

![screenshot-message_template]

Allows you to define the message template using a mixture of **text**, **phpBB tags** (*for example: `[color=red]this text is red[/color]`*), **constants** (*for example: `this script displays metal using the color {COLOR.MET}`*), **variables** (*for example: `the input metal is {m}`*) and **control structures** (*for example: `The output metal is{?M} not{/M} zero`*).

Settings > Import/Export configuration
-------------------------------------------

Allows you to import/export all settings as text (stringified JSON).

[OGame]:http://en.ogame.gameforge.com/
[Firefox]:https://www.mozilla.org/firefox
[Greasemonkey]:https://addons.mozilla.org/firefox/addon/greasemonkey/
[Scriptish]:https://addons.mozilla.org/firefox/addon/scriptish/
[Chrome]:https://www.google.com/chrome/
[Tampermonkey]:https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo
[install link]:https://github.com/EliasGrande/OGameTradeCalculator/raw/master/dist/releases/latest.user.js
[tolerated by OGame Origin]:http://board.origin.ogame.gameforge.com/board175-user-projects/board39-official-tolerated-tools-addons-scripts/4367-ogame-trade-calculator/
[translations]:https://github.com/EliasGrande/OGameTradeCalculator/tree/master/dist/locale
[screenshot-calculator]:https://github.com/EliasGrande/OGameTradeCalculator/raw/master/dist/img/readme/calc.png
[screenshot-ratio_list]:https://github.com/EliasGrande/OGameTradeCalculator/raw/master/dist/img/readme/ratio-list.png
[screenshot-default_values]:https://github.com/EliasGrande/OGameTradeCalculator/raw/master/dist/img/readme/def-values.png
[screenshot-abbreviations]:https://github.com/EliasGrande/OGameTradeCalculator/raw/master/dist/img/readme/abb-auto.png
[screenshot-message_template]:https://github.com/EliasGrande/OGameTradeCalculator/raw/master/dist/img/readme/msg-tpl.png