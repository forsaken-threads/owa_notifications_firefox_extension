Outlook Web App Notifications - Firefox extension
=================

Firefox extension that adds system notifications capability to [OWA - Outlook Web App](https://en.wikipedia.org/wiki/Outlook_Web_App).

The extension is activated if you have an OWA tab open or when you open a new tab and log into OWA. No configuration needed. The extension *doesn't* need any OWA account information, *doesn't* read any private data and *doesn't* connect to the internet to send any data.

How it works: when new email arrives into OWA a system notification about this event will be shown. Also the fav icon and document title of the OWA tab are updated to show the number of unread emails. The fav icon is updated so that you have visual cues when OWA tab is pinned. Document title is updated so that even if Firefox is not the active window, you will see in the taskbar the number of unread emails. This helps in situations when you are not at the computer when new emails arrive and so you don't see the notifications and when you come back you just have to glance over the taskbar to see if there are any unread emails - no need to remember to activate Firefox window to check emails every time you come back to your computer.

How it really works: for each tab open that has the url in the form "http://anything/owa/anything" or "https://anything/owa/anything" a timer task is set to fire every 1 second by default (configurable). The task counts the number of unread emails (using some css selectors) and if the count is different than the last one it updates the fav icon and document title and also if it's greater it shows a notification with the number of new unread emails.

Fork of [OWA_firefox_addon by Phil Baranovskiy](https://github.com/rockfield/owa_firefox_addon).

![Notification when tab is not active](https://raw.githubusercontent.com/mihai-chezan/owa_notifications_firefox_extension/master/doc/tab-normal.png "Notification when tab is not active")

![Notification when tab is pinned and not active](https://raw.githubusercontent.com/mihai-chezan/owa_notifications_firefox_extension/master/doc/tab-pinned.png "Notification when tab is pinned and not active")

![Notification when tab is active](https://raw.githubusercontent.com/mihai-chezan/owa_notifications_firefox_extension/master/doc/tab-active.png "Notification when tab is active")

![Notification when tab is pinned and active](https://raw.githubusercontent.com/mihai-chezan/owa_notifications_firefox_extension/master/doc/tab-pinned-active.png "Notification when tab is pinned and active")

![Notification and browser taskbar when other window is active and in focus](https://raw.githubusercontent.com/mihai-chezan/owa_notifications_firefox_extension/master/doc/taskbar.png "Notification and browser taskbar when other window is active and in focus")

