#  Mastodon Profile redirect

One thing that’s a bit of a hassle with Mastodon is that you can’t immediately follow people on other instances: you have to copy the username and search for it on the instance that hosts your account.

To make this easier, this extension exists. Press the button, and you’ll be taken to the same account as viewed from the Masto instance you are on.

## Attribution 

This is taken from https://github.com/bramus/mastodon-profile-redirect/ and converted into a Safari extension using the process outlined here https://developer.apple.com/documentation/safariservices/safari_web_extensions/converting_a_web_extension_for_safari

I have tested this works on both my iOS and macOS device.

## Installation

These aren't step by step instructions. But rather some pointers in the right direction. As a starting point you need XCode.

### macOS

 1. Make sure that your macOS app is selected in the Scheme menu in Xcode’s main toolbar.
 2. Click the Run button, or choose Product > Run to build and run your app.
 3. Enable your app extension in Safari:
    1. Open Safari and choose Safari > Preferences.
    2. Select the Advanced tab, then select the “Show Develop menu in menu bar” checkbox.
    3. Choose Develop > Allow Unsigned Extensions
    4. Choose Safari > Preferences and click the Extensions tab. T
    5. Find your new extension in the list on the left, and enable it by selecting its checkbox.

### iOS
 
 1. Enable Developer mode on your phone (Settings > Privacy & Security > Developer Mode) and connect your iPhone to your mac usign a cable,
 2. [Add Signing Capabilities](https://developer.apple.com/documentation/xcode/adding-capabilities-to-your-app).
 3. Allow your iPhone to trust your certificate at Settings > General & VPN, DNS & Device Management > Developer App > Trust
 4. Now build your app for your phone:
     1. Make sure that your iOS app is selected in the Scheme menu in Xcode’s main toolbar.
     2. Make sure your iOS device is selected in the Scheme menu in Xcode’s main toolbar.
     3. Click the Run button, or choose Product > Run to build and run your app.
     4. Unlock your iOS device to ensure the installation can complete
 5. Enable the extension in Safari:
    1. Tap the Page Settings button (`AA`) on the left side of the search field, then tap the extension you want to give permissions to.
    2. Choose how much access to give each extension.

## Configuration

 - Make sure you configure the extension once installed. To do this, right click on the extension icon and choose "Manage Extension". Then choose "Preferences"
 - On iOS the Extension settings are at Settings > Safari > Extension >  Mastodon Profile Redirect > Extension Settings
 - When viewing a Mastodon page, hit the icon to get redirected to the profile shown on your instance.
 - Supported pages
    - Profile page
    - Profile page that is set up to redirect to another account
    - Message detail page

## Support and bugs

This project is offered as is. However, I am open to receiving bug reports and accepting PRs to improve this extension.

## License

This project is released under the MIT public license. See the enclosed LICENSE for details.
