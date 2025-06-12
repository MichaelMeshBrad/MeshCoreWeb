## v1.17.0
- added ability to import and export identity key in config backup
- added ability to search nodes on local map and internet map
- added ability to filter nodes on internet map by type, and by those that you uploaded
- added name and public key of user that uploaded internet map nodes to the info popup
- added timestamp of when an internet map node was last updated to the info popup
- added select all and deselect all buttons to config import and export screens
- message notifications no longer open duplicate screen if already viewing that conversation
- notifications are now grouped together, such as dms from the same contact, or messages in the same channel
- managing identity key is now available by default in firmware v1.7.0+
- simplified user experience for filtering local map, and added filter by favourites
- error is now shown when scanning for bluetooth devices fails
- fixed bug where contact icon colours were different on web app
- fixed bug where search bar keyboard would not dismiss when navigating away

## v1.16.2
- https://files.liamcottle.net/MeshCore/v1.16.2/
- fixed bug where my telemetry screen showed grey screen
- force disconnect ble connections after confirming app exit
- force disconnect ble connections when scanning for available devices

## v1.16.1
- fixed bug on ios where contact avatar was on left and name was centered

## v1.16.0
- https://files.liamcottle.net/MeshCore/v1.16.0/
- added ability to set contacts as favourites
- added ability to filter contacts by favourites only
- added ability to view own telemetry from settings screen
- added new "heard x repeats" to channel messages when a repeat is heard by your companion radio
- added view telemetry button to contact details screen for repeaters
- added contact avatar to contact messages app bar and improved app bar text
- added repeater clock from login response to the repeater status page
- added support for new noise floor stats for repeaters and room servers
- added distance between hops to info popup when tapping snr bubble in map path trace tool
- added dynamic contact avatars to discover list
- improved error message popup when clock cannot go backwards
- max channel message length is now calculated based on your device name
- simplified user experience for filtering contacts
- fixed bug where info banner on connect screen would show up as you went to tap screen
- fixed bug where you could enter more text in device name field than firmware would accept
- fixed bug where sending long channel messages would cut them shorter on recipient side

## v1.15.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.15.0+32-025ae5e-release.apk
- added sender name initials and emoji support to channel messages
- added colours, name initials and emoji support to contact list icons
- added button to telemetry screen to auto fetch telemetry every 10 seconds
- added ability to view app change log from about screen
- added ability to configure environment telemetry permissions
- added ability to tap battery percentage in app bar to show voltage
- added ability to turn off message notifications for specific channels
- added icons to advert dropdown menu
- fixed bug where user could set a blank name
- fixed bug where user could set a name with invalid characters
- fixed bug where increasing system font size would make app bar text too large
- fixed bug where telemetry permissions showed wrong contacts count for location permission
- fixed bug where contacts search would not clear when connecting to a different device
- improved bluetooth performance by upgrading internal library
- improved battery percentage calculation by using 3.0volts as 0% instead of 3.4volts
- renamed "Full Events" to "Debug Flags" in repeater and room server status screens
- ui improvements

## v1.14.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.14.0+31-0f7f662-release.apk
- added altitude to telemetry position ui if non zero
- added support for current, power and voltage telemetry types
- added support for temperature, humidity and barometric pressure telemetry types
- added new dropdown to view other telemetry channels
- added new debug logs screen in settings
- added new tab to repeater neighbours to view as a list
- added ability to show contact name labels on repeater neighbours map
- added device info to bottom of settings screen
- added "clear stats" command to repeater commands help
- increased message attempts from 3 to 5 when a direct path is set
- improved contacts sync to help prevent lost contacts

## v1.13.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.13.0+30-bae92a6-release.apk
- added new foreground service to android app to allow device to stay connected when app is minimised
- added new persistent notification to show what device is connected when app is minimised
- added support for updated repeater neighbours response with seconds ago, instead of timestamp
- improved ui for position and telemetry settings screens when they're not supported by connected device

## v1.12.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.12.0+29-88d8ed0-release.apk
- added support for fetching telemetry from contacts (battery and position)
- added new position settings screen to configure gps mode
- added new telemetry settings screen to configure telemetry permissions
- added new contact permissions screen to configure specific contact permissions
- added ability to tap alert popups to dismiss them
- added button to go to contact details screen from local map contact popup
- added button to share contact from contact details screen
- added ability to purge all contacts from settings screen
- added dynamic battery icon to main app bar instead of battery text label
- added ability to change tile layers on all map screens
- added open topo map tile layer
- improved performance of syncing specific contacts when adverts are received or paths change
- fixed bug where ui was hidden under navigation bars on android 15+
- fixed bug where user could choose an invalid custom bluetooth pin
- fixed bug where ble connection was successful but connect screen didn't navigate to main screen
- fixed bug where chat message input was cleared when retrying a failed message
- fixed bug where unsupported map zoom levels caused invalid server requests to tile providers
- fixed bug where internal event listeners would fire in different order and cause lost contacts

## v1.11.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.11.0+28-abda72e-release.apk
- added new settings screen to configure bluetooth pin
- added new screens to import and export companion configuration
- added new zero hop neighbours map to repeater remote management
- added hop count to long press menu for received channel messages
- added warning popup when pinging a contact if multiple contacts have same first byte
- added support for TCP/WiFi connections in Web App https://app.meshcore.nz
- added support for pressing enter to send messages on web (shift+enter to add new line)
- added haptic feedback when long pressing map and messages
- fixed bug where adding contacts manually would set path as direct instead of flood
- increased error message duration from 5 to 15 seconds

## v1.10.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.10.0+27-a371ded-release.apk
- added ability to upload contacts to internet map
- added ability to see radio settings when tapping nodes on internet map
- added ability to update own radio settings to those used by a node on internet map
- added marker clustering support to local and internet maps to improve ux and performance
- added new contact settings screen
- added new setting to enable/disable auto adding contacts from adverts, requires firmware v1.5.0
- added new discover screen that shows recently received adverts, requires app to be connected when advert is received
- added ability to add contacts from discover screen
- added ability to activate premium features without an internet connection
- added distance away in contact details screen

## v1.9.1
- https://files.liamcottle.net/MeshCore/MeshCore-v1.9.1+26-9e7527c-release.apk
- fixed bug where timestamps for outgoing messages showed the wrong date

## v1.9.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.9.0+25-f8c6c47-release.apk
- added new screen to view contact details
- added new screen to manage auto advert intervals for repeaters and room servers
- added ability to long press path trace map to set self position
- added ability to add and remove your companion node on the internet map
- added ability to zero hop ping repeaters and room servers from contacts list
- added ability to connect to usb companion on the web app
- timestamp under messages now shows sender timestamp instead of received timestamp
- fixed bug where keyboard would not dismiss when saving repeater and room server settings
- fixed bug where send button in os keyboard would not send cli command
- fixed ble connections to esp32 devices in web client

## v1.8.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.8.0+24-6639c50-release.apk
- added confirmation dialog before exiting app when connected to a device
- added support for running app from web browsers
- long pressing contact messages now shows the timestamp the sender sent it at
- increased timeouts for cli commands and remote management advert buttons
- refactored internal database handling to only allow one database instance at a time
- fixed bluetooth bug where device would try to auto reconnect even if pairing failed

## v1.7.1
- https://files.liamcottle.net/MeshCore/MeshCore-v1.7.1+23-f7363b6-release.apk
- fixed bug where it wasn't possible to reboot esp32 devices when ble write without response was not supported
- fixed bug where repeaters layer was not selected by default in the trace path map screen
- fixed bug where negative snr values in trace path map, and list would show as 50dB+

## v1.7.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.7.0+22-f092beb-release.apk
- added new tools section in main menu
- added new internet map screen to view publicly shared meshcore nodes (requires internet connection)
- added new path tracing feature, to view snr for each repeater hop (requires firmware v1.4.0+)
- added mutex lock to contact sync to prevent race condition causing contacts to get deleted
- added mutex lock to message sync to prevent race condition causing duplicate messages
- added room server status tab, currently for admins only, will need ui adjustments for guest access
- battery level is now fetched as soon as connected instead of waiting for contacts sync
- fixed bug where bluetooth would not auto reconnect if a previous reconnect failed
- fixed bug where removing an entry in custom path would remove all the commas
- fixed bug where keyboard would show when navigating back, if the field didn't have focus
- fixed margins on alert popups

## v1.6.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.6.0+21-fac7e35-release.apk
- added ability to share and scan contact qr codes
- added ability to view known repeaters for custom paths
- added button to remove specific repeater from custom path
- added new unique colours based on contact name for channel messages
- added button to show remembered password for repeater and room server login
- added unread message indicator to contact and channel tabs
- ui improvements for sharing contacts, and other menu cleanups
- fixed bug where qr codes where black in dark mode and could not be seen

## v1.5.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.5.0+20-86a8e10-release.apk
- NOTE: custom channels requires v1.3.0+ companion firmware
- added ability to create custom channels, which can be used for secure, mesh wide group chats
- added ability to add and share channels via qr code
- added ability to quickly add the public channel
- added option to order contacts list by most recent messages first
- added new menu to radio settings section, to allow picking from suggested radio settings
- added filter menu to search bar to select room servers when selecting path contacts
- added new satellite map tile layer from esri
- added attribution overlay for map tile providers
- decreased the size of the floating buttons on the map
- fixed some ui issues where small screens would not scroll down

## v1.4.1
- https://files.liamcottle.net/MeshCore/MeshCore-v1.4.1+19-b98b156-release.apk
- added button to send message to a room server from the map screen
- implemented new companion protocol version to allow for showing received message snr
- when a message is received with snr information, it can be seen by long pressing the message
- duplicate messages are no longer shown when a senders retry is received for an existing message
- confirmation dialog buttons for deleting messages are now red and show on the right side
- fixed bug where contacts would disappear when a corrupted name was received

## v1.4.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.4.0+18-679dde8-release.apk
- added last snr to repeater stats screen
- added new notification when a new contact is discovered
- added new notification settings screen to adjust preferences
- added auto retry of failed direct messages up to 3 attempts
- added message settings page to configure if last send attempt should send as flood
- added start ota command to repeater commands help list
- added info banner to manage identity screen to say custom firmware is needed
- contacts are now ordered most recently heard by default
- room server remote management screen now defaults to showing the settings tab
- improved error message when failing to connect to a half bonded ble device
- fixed bug where some unread message counts were showing incorrect values

## v1.3.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.3.0+17-07452fd-release.apk
- added ability to send and receive room server messages
- added ability to view locally cached room server messages without a connection to room server
- added remote management support for room servers, command line and form based
- added notifications for new room server messages
- both sent and received timestamps for incoming room server messages are now shown in long press menu
- unread messages badge is now shown for room servers in contacts list
- devices with new v1.0.0+ firmware versions now show at bottom of settings page
- fixed some help entries in the repeater commands list

## v1.2.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.2.0+15-549c99d-release.apk
- added new repeater settings page
- added ui to configure repeater name and radio settings
- added ui to set admin and guest password for repeaters
- added ui to set repeater position
- added button to sync repeater clock from current device
- added buttons to advert, sync clock and reboot repeaters via remote management
- added checkbox to remember admin password per repeater
- added info banner with default bluetooth pin on connect screen
- added new position selector screen to pick lat lon by tapping on map
- switched to using full keyboard layout for number inputs as some regions don't show dot for decimal inputs

## v1.1.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.1.0+14-2802f4e-release.apk
- added ability to log in to a repeater as an admin or a guest
- added ability for guests to view status of repeaters
- added new remote management feature for repeater admins
- added new quick commands help section to repeater management menu
- added button to remote manage repeaters from map popup menu
- added path to contact name subtitle when clicking a contact on the map
- fixed bug where adding a new contact would always add as chat, regardless of the contact type you selected
- other ui improvements

## v1.0.9
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.9+13-6091dd6-release.apk
- added red indicator icon to filter button when selected filters don't include all results
- contact search bar now shows how many contacts are in the list, based on selected filters
- fixed bug where app would not disconnect from BLE device when pairing fails, causing device to no longer be discoverable
- internal improvements to bluetooth connection handling
- increased connection timeout for fetching device info
- please upgrade to the latest firmware for the best experience
- ble devices are now manually bonded before trying to use them

## v1.0.8
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.8+10-a291a52-release.apk
- added ability to filter contact types on map
- added ability to manually create contacts from a known public key
- added menu to advert button to show more options
- added button to export self advert to clipboard
- added icon for room servers
- contacts list now uses the local timestamp of when a contact was last heard
- fixed bug where private key field was not editable when managing identity key
- fixed bug where it wasn't possible to enter decimal point and minus sign in some settings fields
- fixed bug where transmit power was not saved when saving device settings

## v1.0.7
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.7+8-8373e33-release.apk
- added ability to filter contacts list by type
- added device model and firmware build info to bottom of settings screen
- added link to meshcore website in about page
- clicking notifications will now open the relevant conversation
- fixed bug where unread messages badge would not update after connecting to different devices
- fixed bug where date was not showing for adverts that are not today

## v1.0.6
- updated android package name to com.liamcottle.meshcore.android
- fixed button to copy public key from map menu
- added required plist values for ios app store

## v1.0.5
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.5+6-1fe395e-release.apk
- added new map feature
- added new about screen to main menu
- added ability to paste comma delimited lat/long into device settings page
- added ability to update device position by long pressing on the map
- all known contacts that have a valid position will be shown on the map

## v1.0.4
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.4+5-3c46b65-release.apk
- fixed issues where lat/long inputs in settings would not show decimal places
- moved disconnect button to top of main screen menu
- added ability to import and export private identity key when firmware has feature enabled
- improved internal contacts management
- direct messages screen now shows how many hops away the contact is
- added contact dropdown menu to messages screen
- added button to clear path input field
- added ability to order contacts alphabetically or by heard recently

## v1.0.3
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.3+4-393e85c-release.apk
- added contact search
- added contact import from clipboard
- added buttons to export contact to clipboard
- add button to copy contact public key
- add button to share contact as zero hop advert
- added public key to settings page, with button to copy
- can now long press messages to view additional actions
- added button to retry failed messages
- added ability to set custom path for contacts
- can select repeaters when setting custom path
- fixed bug with header changing colour on scroll
- adjusted theme colours for floating action buttons

## v1.0.2
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.2+3-0fb2a75-release.apk
- Added Dark Mode (automatic based on device theme)

## v1.0.1
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.1+2-e80c9f4-release.apk
- added support for automatically reconnecting to device when it comes back into range.
- this is provided the app has not been killed. for now, if you force quit the app, you will need to manually connect on launch

## v1.0.0
- https://files.liamcottle.net/MeshCore/MeshCore-v1.0.0-release.apk
- initial release
