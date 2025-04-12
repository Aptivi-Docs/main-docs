---
description: Not all versions of libraries are supported.
icon: question
---

# Support Periods

{% hint style="info" %}
List of eligible libraries and applications:

* Nitrocid KS
* Terminaux
* BassBoom
{% endhint %}

When a library is released, it typically comes with just one version series, which is typically 1.x or 0.1.x. When the second series starts, such as 2.x or 0.2.x, the support period for all versions in the series will be in the following form:

* **Projects that reached 1.x or later**
  * The following support periods, which start with the release date of the last sub-series released (such as Terminaux 5.4.x) before the next major series (6.x.x), are as follows:
    * One-year window is applied to projects that get updated frequently in major versioning, such as Terminaux.
    * Two-year window is applied to projects that get updated frequently in minor versioning, such as Textify.
    * Three-year window is applied to projects that get updated occasionally in an unplanned schedule, such as SpecProbe.
* **Projects that are in the 0.x.y series**
  * The following support periods, which start with the release date of the last sub-series released (such as Terminaux 5.4.x) before the next major series (6.x.x), are as follows:
    * Six-month window is applied to projects that get updated frequently in major versioning.
    * One-year window is applied to projects that get updated frequently in minor versioning.
    * Two-year window is applied to projects that get updated occasionally in an unplanned schedule.
* **Projects that are in the 0.0.x.y series**
  * There is no support for these versions except the latest version, which won't last long. As soon as the library or the application moves to the 0.x.y series or the x.y.z series, none of the 0.0.x.y series will be in support.

{% hint style="info" %}
When a beta version of a specific version series is announced, the beta versions are supported through the lifetime of the testing period, explicitly (with a set release date announced) or implicitly (no announcement), until the first public release of the version, after which all beta versions under that version circle are assumed to be expired.

For example, Nitrocid KS 0.0.6 had a beta testing period that lasted 6 versions (0.0.5.9 -> 0.0.5.14) until the first public release.
{% endhint %}

However, applications and libraries may have different support periods, which are listed below:

* [**Nitrocid KS**](https://app.gitbook.com/s/yhORwVwuIgJMLsQRqN3S/versions-and-compatibility/supported-versions)
  * Short term releases: 9 months as of 0.1.1 or later
  * Long term releases: 5 years of non-security fixes, and 5 years of security and critical fixes
  * Although Windows 10 is still supported until October 15th, 2025, we **no longer support** running Nitrocid KS on Windows 10 beginning February 27th, 2025.

## Current support periods

Only libraries and applications that don't have their own support policy are shown here.

* **Terminaux**
  * 4.3.x series are supported until July 7th, 2025.
  * 5.4.x series are supported until September 26th, 2025.
  * 6.1.x series are supported until August 5th, 2026 (6 extra months after February 6th, 2026 due to buggy release of 6.0.0).
* **BassBoom**
  * 0.1.x.y series is supported until May 31st, 2025.
  * 0.2.x.y series is supported until the 1.x version of BassBoom is released, which will accompany with the 1.x version of a future BassBoom library under a separate library.

## Operating system support

When it comes to supporting operating systems in our apps, the below support dates will override the above main support dates. Here are the current states:

### Windows

| Version    | Support   | End of support      |
| ---------- | --------- | ------------------- |
| Windows 11 | Supported | December 16th, 2032 |
| Windows 10 | Supported | December 17th, 2026 |

### macOS

| Version            | Support   | End of support   |
| ------------------ | --------- | ---------------- |
| macOS 15 (Sequoia) | Supported | To be determined |
| macOS 14 (Sonoma)  | Supported | To be determined |
| macOS 13 (Ventura) | Supported | To be determined |

### Linux

We support running our applications on Linux distributions, as long as both the corresponding .NET runtime, which is used to run our apps, and the distribution itself are supported. End of life versions and/or distributions are not supported.

### Others

We don't provide support for other operating systems.
