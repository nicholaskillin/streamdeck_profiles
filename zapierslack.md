## Overview
The Stream Deck buttons for controlling Slack are just simple "open website" buttons. The URL, however, is link to a Zapier webhook. I use Zapier to automate a few things. Here's what my "Break" button looks like:

[![Screen_Shot_2018-09-24_at_4.24.21_PM.png](https://i.postimg.cc/rmcwVmMz/Screen_Shot_2018-09-24_at_4.24.21_PM.png)](https://postimg.cc/67jXzB7N)

### Step One — Catch Hook
Zapier will generate a webhook URL. Copy it:
[![Screen_Shot_2018-09-24_at_4.27.07_PM.png](https://i.postimg.cc/x8DhDJ2F/Screen_Shot_2018-09-24_at_4.27.07_PM.png)](https://postimg.cc/G8Kqvp9k)

### Step Two — Format Date/Time
This part is optional. If you want to tell Slack to go online or away immediately, you don't need to mess with times. However, if you want to go on break and have your Slack status show what time you'll be back, you'll need to format the time. 

Under **Transform**, select "Add/Subtract Time". For values **Input**, choose "Zap Meta Human Now." What does that mean? Nobody knows, but it'll work. Trust me.

**Expression** should be set to +15m to add fifteen minutes (for a break). You can put +1h to add an hour for lunch.

**To Format** needs to be set to "Use a Custom Value (advanced)." and lastly, you'll set **Custom Value for To Format** to `h:mmA`.

Click Continue.

### Step Three — Action
When setting your Slack Status, you'll have three options. Here's what to make it look like for your break:

[![Screen_Shot_2018-09-24_at_4.34.38_PM.png](https://i.postimg.cc/8czKVhY4/Screen_Shot_2018-09-24_at_4.34.38_PM.png)](https://postimg.cc/r07C1tMR)