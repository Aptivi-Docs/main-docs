---
icon: question
description: Not all versions of libraries are supported.
---

# Support Periods

{% hint style="info" %}
List of eligible libraries and applications:

* Nitrocid KS
* Terminaux
* BassBoom
{% endhint %}

When a library is released, it typically comes with just one version series, which is typically 1.x or 0.1.x. When the second series starts, such as 2.x or 0.2.x, the support period for all versions in the series will be in the following form:

* **Libraries that reached 1.x or later**
  * Support period starts from the date of the first series released in a year and a month until 2 years, and all other versions except the last one prior to the next version series development are automatically assumed to be EOL when the next version series is released, just like the below example:
    * 1.x is out in August 2025 and will reach EOL in September 2027.
      * 1.1.x is out in August 2025, and has reached EOL because 2.x was out on January 2026.
      * 1.2.x is out in November 2025, and hasn't reached EOL because it was the last version in the series, and will reach EOL in September 2027.
    * 2.x is out in January 2026 and will reach EOL in February 2028.
      * and so on...
    * 3.x is out in November 2026 and will reach EOL in February 2028.
      * and so on...
* **Libraries that are in the 0.x.y series**
  * Support period starts from the date of the first series released in a year and a month until one year, but with no last version policy as mentioned above, just like the below example:
    * 0.1.x is out in August 2025 and will reach EOL in September 2026.
    * 0.2.x is out in January 2026 and will reach EOL in February 2027.
    * 0.3.x is out in November 2026 and will reach EOL in February 2027.
* **Libraries that are in the 0.0.x.y series**
  * There is no support for these versions except the latest version, which won't last long. As soon as the library or the application moves to the 0.x.y series or the x.y.z series, none of the 0.0.x.y series will be in support.

{% hint style="info" %}
When a beta version of a specific version series is announced, the beta versions are supported through the lifetime of the testing period, explicitly (with a set release date announced) or implicitly (no announcement), until the first public release of the version, after which all beta versions under that version circle are assumed to be expired.

For example, Nitrocid KS 0.0.6 had a beta testing period that lasted 6 versions (0.0.5.9 -> 0.0.5.14) until the first public release.
{% endhint %}

However, applications and libraries may have different support periods, which are listed below:

* [**Nitrocid KS**](https://app.gitbook.com/s/yhORwVwuIgJMLsQRqN3S/versions-and-compatibility/supported-versions)
  * Short term releases: 9 months as of 0.1.1 or later
  * Long term releases: 5 years of non-security fixes, and 5 years of security and critical fixes

## Current support periods

Only libraries and applications that don't have their own support policy are shown here.

* **Terminaux**
  * 4.3.x series are supported until September 1st, 2026.
  * 5.4.x series are supported until September 1st, 2026.
* **BassBoom**
  * 0.1.x.y series is supported until June 1st, 2025.
  * 0.2.x.y series is supported until June 1st, 2025.
