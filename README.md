# Android-CountUpTimer
##Description
A count up timer that can be used in Android. The class has features:
1. Pause
2. Restart

##Install
1. Download the class CountUpTimer. (pull the repository)
2. Put the class into your package.
3. Change the package name from null to your package name.

##Usage
```java
CountUpTimer timer = new CountUpTimer(TOTAL_TIME, TICK, new CustomTimer.TimerDelegate() {
            @Override
            public void onTick(long millisUntilFinished) {
                // do anything you want
            }

            @Override
            public void onFinish() {
            //do anything you want
            }
        });
        timer.start();
        timer.pause();
        // the start call is used for starting and resuming
        timer.start();
        long milliSecondsLeft = timer.getTimeToGo();
        // restart method: restarts the timer.
        timer.restart();
        String currentTime = timer.getTimeString();
```
##TODO
* [x] Add a method that returns a string representation of the timer.
* [x] Add a restart method that restarts the timer with the initial settings.
* [ ] Add a pause method that pauses the timer for a given amount of milliseconds.
* [ ] Add a view (subclass of textview) that the timer updates each tick.
* [ ] Make this a gradle project.
