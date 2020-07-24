## Update add-ons for Thunderbird 78 using wrapper APIs

Thunderbird 78 usually requires significant changes to add-ons, such as the locale and preference system as well converting XUL documents to HTML. Furthermore, the new WebExtension technology does not yet provide all the functions which are available to add-ons by using legacy Thunderbird APIs.

To support developers, we created these wrapper APIs which do not require all of these changes, just to get the add-on running in Thunderbird 78 again. The goal is to get as many add-ons compatible with the current ESR version, so the users can continue to work with their beloved add-ons.

| API             | Description |
| --------------- | ----------- |
| [BootstrapLoader](https://github.com/thundernest/addon-developer-support/wiki/Using-the-BootstrapLoader-API-to-convert-a-Legacy-Bootstrap-WebExtension-into-a-MailExtension-for-Thunderbird-78)      |  Update a Legacy Bootstrap WebExtension (draft)
| [WindowListener](https://github.com/thundernest/addon-developer-support/wiki/Using-the-WindowListener-API-to-convert-a-Legacy-Overlay-WebExtension-into-a-MailExtension-for-Thunderbird-78)      |  Update a Legacy Overlay WebExtension

_Please note: Updating with these wrapper APIs should only be the first step, as it is an [experimental API](https://thunderbird-webextensions.readthedocs.io/en/latest/how-to/experiments.html) which is only a temporary solution. We encourage and try to help add-on developers to continue the upgrade process to a pure MailExtension. After the initial conversion we will create little "rainy day" update guides, to get the legacy components out piece by piece._
