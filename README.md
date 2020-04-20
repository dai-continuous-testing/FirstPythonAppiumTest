# Mobile Automation using Appium and Python programming language.

This project demonstrates Mobile Automation using Appium and Python programming language.
Pycharm IDE used for Python.

Project is associated with the blog - Complete Guide Appium Testing using Python - https://experitest.com/appium-testing/the-complete-guide-appium-testing-using-python

This example will cover:

Basic Test case creation using Python/unittest framework using Appium Python Library/Appium Server.

### Steps to run demo test

1. Clone this git repository

	```
	git clone
	```

2. Start Appium Server using Appium Desktop installed in your PC.
   The project expects the Appium Server to run on localhost:4723. If you run the server to different host and port. Please change the code.

3. Download the Eribank application using URL : https://experitest.s3.amazonaws.com/eribank.apk to c:\\  (The code uses the Application from c:\\ (in windows). Please change the code in case you   change the download location)

4. Import the cloned project in Pycharm (In Pycharm menu, navigate to File > Open or "Open" if no projects are open)

5. Modify following variables in the code if necessary

   Open **AppiumTest.py** and modify following if necessary,

      Appium Server listening host and port.

      ```
      self.driver = webdriver.Remote("http://localhost:4723/wd/hub",self.dc)
      ```

      Path of the Eribank application (in case downloaded location is different)

      ```
      self.dc['app'] = "c:\\eribank.apk"
      ```

      Device name (After excecuting adb devices. See "Android device recognition" in the blogs)

      ```
      self.dc['deviceName'] = 'a3ae1c63'
      ```


5. To know how execute the test, (Associated blog link - https://experitest.com/appium-testing/the-complete-guide-appium-testing-using-python)
      * Make sure you set the Interpreter, Please follow "Interpreter Configuration" in the blog.
      * Make sure you have imported Appium Dependency, Please follow the "Creating First Test using Appium and Python" in the blog.
      * Please follow the section "Executing the Test".

