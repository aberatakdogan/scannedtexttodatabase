
In this method, I am trying to get text from a scanned picture in Java programming language for a mobile application.

Although I can observe the scanned text in my app, I also want to keep these text data on a database system using Firebase Realtime Database solution.

When I run my app with these method, I encountered the error message as below.

How can I solve this error or is there any way to save my data to the Realtime Database?

-----------------------------------------------------------------------------------------
E/AndroidRuntime: FATAL EXCEPTION: main
    Process: com.example.myapplication, PID: 28303
    java.lang.RuntimeException: Failure delivering result ResultInfo{who=null, request=203, result=-1, data=Intent {  launchParam=MultiScreenLaunchParams { mDisplayId=0 mBaseDisplayId=0 mFlags=0 }(has extras) }} to activity {com.example.myapplication/com.example.myapplication.MainActivity}: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.String com.google.firebase.auth.FirebaseUser.getUid()' on a null object reference
        at android.app.ActivityThread.deliverResults(ActivityThread.java:4520)
        at android.app.ActivityThread.handleSendResult(ActivityThread.java:4563)
        at android.app.ActivityThread.-wrap22(ActivityThread.java)
        at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1698)
        at android.os.Handler.dispatchMessage(Handler.java:102)
        at android.os.Looper.loop(Looper.java:154)
        at android.app.ActivityThread.main(ActivityThread.java:6776)
        at java.lang.reflect.Method.invoke(Native Method)
        at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:1496)
        at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1386)
     Caused by: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.String com.google.firebase.auth.FirebaseUser.getUid()' on a null object reference
        at com.example.myapplication.MainActivity.getTextFromImage(MainActivity.java:144)
        at com.example.myapplication.MainActivity.onActivityResult(MainActivity.java:104)
        at android.app.Activity.dispatchActivityResult(Activity.java:7280)
        at android.app.ActivityThread.deliverResults(ActivityThread.java:4516)
        at android.app.ActivityThread.handleSendResult(ActivityThread.java:4563) 
        at android.app.ActivityThread.-wrap22(ActivityThread.java) 
        at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1698) 
        at android.os.Handler.dispatchMessage(Handler.java:102) 
        at android.os.Looper.loop(Looper.java:154) 
        at android.app.ActivityThread.main(ActivityThread.java:6776) 
        at java.lang.reflect.Method.invoke(Native Method) 
        at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:1496) 
        at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1386) 
