---
description: >-
  Learn how to disable bad state tracking for Windows to avoid random
  disconnections
icon: wifi-slash
---

# Fix Windows random disconnections

Network Bad State Tracking for Windows has been implemented in Windows 10 and higher. It allows your computer to automatically disconnect your Internet connection, reset the network adapter, and reconnect to your network when your connection is poor or limited. However, this feature is not fool-proof, as it also causes your computer to randomly disconnect from the Internet when you're downloading a huge file at full speed, it can't reach the "network check" servers, and your connection is in a state where it needs resetting, though it doesn't happen as often.

The reason that Windows continuously pings the "network check" servers is that because it needs to know whether you're connected to a network that has access to the entire Internet or not. If it can't reach those servers, then this means that you have limited connectivity.

{% hint style="info" %}
This pinging is not the only reason why Windows randomly disconnects your computer from the Internet. There can be many factors of random disconnection, such as outdated device drivers, loose connection to the Wi-Fi adapter, faulty adapter, or, in case of USB dongles, either a faulty USB Wi-Fi dongle or a faulty port.
{% endhint %}

We've implemented a small tool for Windows that allows you to turn off this kind of check to avoid random network disconnections when you're trying to download a huge file at full speed, called NetLimDisable, that is [fully transparent](https://github.com/Aptivi-WPT/NetLimDisable) about the process. It checks for the value of `HKLM\SOFTWARE\Microsoft\WcmSvc\EnableBadStateTracking` in the Windows registry.

* If this value is omitted from the `WcmSvc` key, Windows enables bad state tracking by default.
* If this value is set to `1`, Windows enables bad state tracking.
* If this value is set to `0`, Windows disables bad state tracking.

To use this program, follow these steps:

1. Go to the [releases](https://github.com/Aptivi-WPT/NetLimDisable/releases) page
2. Download the binary ZIP file and extract it
3. Open the `NetLimDisable.exe` file (requires UAC to be granted)
4.  Check or uncheck the checkbox that is shown in the below window:\


    <figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
5.  Click on Apply, and you should see this dialog box declaring that the operation succeeded:\


    <figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
6.  (Optional) Open the registry editor (`Windows + R` -> `regedit.exe` -> `ENTER`), open the above registry key, and verify that `EnableBadStateTracking` is set to `1` or `0`.\


    <figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
7. Continue your operation.

{% hint style="info" %}
If you're still experiencing connection drops, restart your computer and try to perform the same operation.
{% endhint %}
