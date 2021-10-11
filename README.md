# Home Automation FAQ

I was so frustrated after the initial week of automating my home that decided to summarize my frustration in a concise set of advices for new automators out there. Hope it saves you some time.

## The things I wish I knew before diving into HomeKit Automation

1. Early accept necessity of hubs / gateways. Most devices on the market require them to function properly. This means if you have a large house with solid walls, each room would require a hub ($10-50 depending on brand), as low-energy protocols such as BLE or Zigbee do not penetrate walls as good as Wi-Fi (which you should not be using anyway, see #3).

2. Whenever you have a choice, stick to Gizbee-based devices. Easier to setup, more reliable and less maintanance in the long run. Not sure what Gizbee is? Google "[Gizbee BLE mesh vs Wi-Fi](https://www.google.com/search?q=Gizbee+BLE+mesh+vs+Wi-Fi)". Sometimes you'd have a BLE device -- make sure you set it up to communicate via a hub and not directly with your phone, as none of your automations will work reliably (or at all) w/o a hub / gateway. In other words, do not allow your "smart app" to use Bluetooth after you paired a device to the hub.

3. Avoid buying Wi-Fi-based devices at all cost, unless you want to spend a day and $$$ re-designing your entire wireles home network. Wi-Fi was not designed for IoT and it's a beginners' delusion to think that since you have a Wi-Fi router already that works fine for your phones and PCs, adding up "smart" devices to your network will be easy. Actually it's 100% opposite, since most of "smart" devices use very dumb Wi-Fi chips and if your home network is anything less than perfect it is __guaranteed__ to give you hours of frustration with the same outcome: it won't work until you get rid of cheap / old routers, split your 2.4 GHz and 5 GHz networks, disable repeaters etc etc. The easier your Wi-Fi setup is the better it is for home automation, period ([more info](https://www.reddit.com/r/HomeKit/comments/bi0bp1/no_response_a_constant_irritation_with_homekit/)).

4. If using Homekit (which is very well integrated, designed and thought thru despite initial UI confusion) you __must__ install and get used to Homebridge as early as possible. Steep, but short learning curve will save you lots of trouble down the way. This means you have to get either Raspberry or HOOBS or ATHOM device, better with Zigbee and Bluetooth modules attached.

5. "Works with HomeKit" label means almost nothing at this point. Very few accessories are trouble-free despite having a HomeKit logo on them. Use Homebridge for everything and before buying something new always check if there's a plugin for your device, not just particular brand -- the particular device you have in mind! Otherwise you'll end up with a crazy zoo of Chinese re-skinned "smart apps", each of them requiring a separate account, "calling home" all the time etc.

6. Homebridge being community driven is also far from perfect, so have your expectations in check, but at least it gives you very good degree of control. Principle advice: enable debug logging and never turn it off. It will save lots of time trying to figure out why something does not work despite lack of error messages. 

7. Forget about using YouTube for research prior buying new gadgets, as almost nobody there talks about real problems you'll face with your bright new colored bulb that drops off the network for now reason and requires 15 minutes to be readded back. Extensively search Reddit and Github to estimate amount of headache that comes with each device. This is true about each and every brand out there even for seemignly easiest devices such as switches, sensors or lamps. The problems stem from Chinese origin of most of the software and hardware: full of bugs that will never be fixed, terrible UI/UX and non-existant English supprt. Best known brands such as Phillips or IKEA are more reliable, but they have limited range of products, so at some point you'd have to swallow the pill and resort to AliExpress. 

99. Remember to ask yourself "Should I do it?" instead of "Can I do it?" Yes, you __probably__ can control your TV from your phone, but do you really need it if there's a perfectly designed remote nearby? 

![You were so preoccupied with whether or not you could that you didn't stop to think if you should.](https://wrnr.com/assets/images/Bobby%20Blogz/2019/march/you-were-so-preoccupied-with-whether-or-not-you-could-you-didnt-stop-to-think-if-you-should.jpg)


