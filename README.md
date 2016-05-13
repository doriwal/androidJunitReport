# androidJunitReport

This project is a fork of http://zutubi.com/source/projects/android-junit-report/

I created this fork as zutubi didnt worked for me for android 4+

This project allows to listen from the device without IDE or ADB connection to JUNIT tests (regardless if its junit/espresso or any other junit freamwork) , and save the test result as junit.xml file in the device.

In order to use it you need to 

1) build with gradle , the output is an android aar 

2) unzip the aar folder , copy the classes.jar , rename it as you wish 

3) add the jar as a dependency to your android application that you are testing 

4) in the application manifest replace the default AndroidJunitRunner with 

instrumentation android:name="com.dw.android.junit.report.JUnitReportRunner" android:targetPackage="XXX""