---
description: >-
  dateparser is a natural language date/time parser for OutSystems applications.
  See below for the wide variety of formats dateparser will parse.
---

# dateparser

### Installation

You can install dateparser from the OutSystems Forge component page:\
[https://www.outsystems.com/forge/component-overview/1385/outsystems-ui](https://www.outsystems.com/forge/component-overview/1385/outsystems-ui)

### Public API

*   ![ServiceAPIMethod](https://ik.imagekit.io/antunes/os-resources/tr:w-18,h-18/ServiceAPIMethod.png) **Parse**&#x20;

    _Attempts to parse a string into a DateTime (exceptions are raised)._

    * ![InputParameter](https://ik.imagekit.io/antunes/os-resources/tr:w-18,h-18/InputParameter.png) **String** _(Text, Mandatory)_
    *   __![InputParameter](https://ik.imagekit.io/antunes/os-resources/tr:w-18,h-18/InputParameter.png) **Type** _(Integer)_&#x20;

        _Past = -1, Future = 1, None = 0_
* ![ServiceAPIMethod](https://ik.imagekit.io/antunes/os-resources/tr:w-18,h-18/ServiceAPIMethod.png) **TryParse**
  *   ![InputParameter](https://ik.imagekit.io/antunes/os-resources/tr:w-18,h-18/InputParameter.png) **String** _(Text, Mandatory)_

      _e.g.: may 27th_
  *   ![InputParameter](https://ik.imagekit.io/antunes/os-resources/tr:w-18,h-18/InputParameter.png) **Type** _(Integer)_

      _Past = -1, Future = 1, None = 0_

### Examples

dateparser can parse a huge variety of date and time formats. Following is a small sample of strings that will be properly parsed. Parsing is case-insensitive and will handle common abbreviations and misspellings.

**Simple**

* last friday at 20:00 ([try it](https://miguel-antunes.outsystemscloud.com/dateparserDemo/Demo?s=thursday))
* last week tuesday
* tomorrow at 6:45pm
* afternoon yesterday
* thursday last week

**Complex**

* 3 years ago
* a year ago
* 5 months before now
* 7 hours ago
* 7 days from now
* 1 week hence
* in 3 hours
* 1 year ago tomorrow
* 3 months ago saturday at 5:00 pm
* 7 hours before tomorrow at noon
* 3rd wednesday in november
* 3rd month next year
* 3rd thursday this september
* 4th day last week
* fourteenth of june 2010 at eleven o'clock in the evening
* may seventh '97 at three in the morning

**Specific Dates**

* January 5
* 22nd of june
* 5th may 2017
* February twenty first
* dec 25
* may 27th
* October 2006
* oct 06
* jan 3 2010
* february 14, 2004
* february 14th, 2004
* 3 jan 2000
* 17 april 85
* 5/27/1979
* 27/5/1979
* 05/06
* 1979-05-27
* Friday
* 5
* 4:00
* 17:00
* 0800

**Specific Times (many of the above with an added time)**

* January 5 at 7pm
* 22nd of june at 8am
* 1979-05-27 05:00:00
* 03/01/2012 07:25:09.234567
* 2013-08-01T19:30:00.345-07:00
* 2013-08-01T19:30:00.34-07:00
* etc
