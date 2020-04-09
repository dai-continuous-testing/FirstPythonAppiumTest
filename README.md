# Mobile Automation using Appium and Python programming language.

This project demonstrates Mobile Automation using Appium and Python programming language.
Pycharm IDE used for Python.

Project is associated with the blog - Complete Guide Appium Testing using Python - <>

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

4. Modify following variables in the code if necessary
   Open EribankTest.java and modify static variables if necessary,

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


5. To know how execute the test,
      * Open the cloned project in Pycharm (Menu > Open )
      * Please follow the section "Executing the Test" in the blog - <>

