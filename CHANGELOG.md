I try to list the changes i make in this changelog:

#19.11.2020 22:26
- hope you can figure out how to use the configuration :) :
- added support for persisting and loading configurations -> now you can configure everything once as you like, create a configuration.json file, save it in e.g. iCloud and from there you can easily use this file via a widget parameter and don't have to think about reconfiguring everything after updating the script itself
- the new parameter must have the form USE_CONFIG:yourfilename.json (so it starts with USE_CONFIG: and ends with .json. The middle part can be chosen by you)
- tried my best to make this as stylable as possible
- support for dark and light versions of purple and black (can be set automatically)
- you can now set chart color, font color, set own background colors and more
- added x axis label for charts
- did a pretty large code refactoring without function changes
- added support for Homebridge Config UI X Authentication Mode 'none' -> so if you chose 'none' and don't need credentials to show your UI in the browser, you now don't need it for this widget anymore
- new screenshots

#17.11.2020 22:08
- complete overhaul of the section above the updated date and below the title for perfect alignment (now only using stacks and spacers)
- only updated one picture (the main pic on top of readme)
- no functionality changed

#17.11.2020 20:31
- just added a new background color BLUE_TO_RED

#17.11.2020 20:14
- added missing reset of notification state (not critical), so that notifications are fired again after everything was back to normal (e.g. HB down -> notification, HB up again -> reset, HB down -> again notification)
- you can also get notified now when a state changed back to normal (but is disabled by default)
- now if temperature is unknown -> it is not shown at all
- added possibility to ignore plugins, Homebridge or Node.js during checking for updates
  - for plugins, enter their npm name (e.g. 'homebridge-fritz') as string in the given empty array 
  - for Homebridge enter 'HOMEBRIDGE_UTD' and for Node enter 'NODEJS_UTD' in the empty array

#16.11.2020 22:24
- added support for entering credentials via widget parameter
- parameter must have the format like admin,,mypassword123,,http://192.168.178.33:8581
- added some concrete error information that should help setting up the widget

#16.11.2020 20:39
- added support for notifications when some status changed
- supported: Homebridge stopped, Homebridge Update available, Plugin Update available, Node.js Update available
- new screenshots
- added changelog
- some filemanager usage refactoring

#15.11.2020 14:26
- overhaul of the status icons, now not using emoji anymore but SFSymbols
- more handling when some requests return undefined
- new screenshots


#15.11.2020 11:25
- fixed the black text color when user uses light mode (now text is always white)
- added unknown status if API requests return undefined
- now user can choose between default purple background and a black background
- now user can set the icons used at a central spot


#14.11.2020 21:44
- added possibility to switch the file manager to local via a variable


#14.11.2020 21:26
- added support to show temperature in Fahrenheit
- more version infos


#14.11.2020 20:48
- just added some infos about the versions of all the systems


#14.11.2020 20:36
- fixed a critical bug (forgot to include the logic for node.js UTD)


#14.11.2020 18:16
- initial commit of the first version of the script