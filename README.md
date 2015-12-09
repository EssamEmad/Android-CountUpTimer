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
```
##TODO
1. Add a method that returns a string representation of the timer.
2. Add a pause method that pauses the timer for a given amount of milliseconds.
