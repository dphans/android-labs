# Network and CPU performance monitor #


NetMeter allows to trouble-shoot performance problems by letting the user see network and CPU usage over time. On a mobile device, battery power is one of the most critical resources. Unexpected heavy network and CPU usage could be indicative power consuming background activities.

![http://android-labs.googlecode.com/svn/trunk/screenshots/netmeter1.png](http://android-labs.googlecode.com/svn/trunk/screenshots/netmeter1.png)


To allow monitoring while doing some other activity, NetMeter can keep running in the background while continuing to collect measurements. Whenever NetMeter is active, a small blue graph icon can be seen in the notification bar, by which it can always be launched again into the foreground. Use "stop" from the menu to close down NetMeter and stop the data collection. The "reset" menu option will reset the cumulative network usage counters in the tabular display part of the screen, without affecting the usage history graph. By default, the history graph shows the maximum amount of available data (max 24h) since NetMeter has been started. Use the "toggle scale" menu option to switch between shorter, more detailed views of the recent past.

![http://android-labs.googlecode.com/svn/trunk/screenshots/netmeter2.png](http://android-labs.googlecode.com/svn/trunk/screenshots/netmeter2.png)

## Finding out which apps consume CPU ##
To see a detailed breakdown of CPU utilization by tasks, use the "show tasks" menu option. It will show which processes in the Android platform have been using CPU during the last 30s and how much. Android does not allow applications to terminate other application processes - this is part of its security model. The Android framework itself manages processes and other OS resources transparently based on application demand. Terminating a process would simply result in it being restarted again if the application still requests to run. Android provides great power and flexibility to application developers, like installing application services to run completely in the background. The only way at this point to deal with application which put an undue strain on resources is to stop them - if the allow to do so, or otherwise uninstall them and contact the developer about providing a more resource efficient implementation.

![http://android-labs.googlecode.com/svn/trunk/screenshots/netmeter3.png](http://android-labs.googlecode.com/svn/trunk/screenshots/netmeter3.png)

## Impact and limitations ##
Measuring detailed CPU utilization is in itself a resource consuming process. Therefore NetMeter itself is likely to show up towards the top of the list of CPU consuming tasks. However once stopped, NetMeter no longer consumes any resources. The history of measurements are kept in memory only by the NetMeter background process. If the phone runs low on memory - the Android platform may decide to stop and restart the process at any time, which will erase the accumulated history and start collection afresh.


NetMeter is primarily intended as an interactive diagnostic tool and not as a long-term network usage counter. For that purpose applications like NetCounter are a better fit.


For more updates, see Android related entries on my [blog](http://blog.kugelfish.com/search/label/Android) and for any comments or questions please contact android@kugelfish.com.