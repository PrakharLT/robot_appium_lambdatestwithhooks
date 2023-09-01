# LT-robot-framework

## Setup
* Clone the repo
* Install dependencies  `pip install robotframework`  &&  `pip install --upgrade robotframework-seleniumlibrary`
* `pip install robotframework-pabot` -> This is for parallelization 
* For Appium, `pip install robotframework-appiumlibrary` .For more information refer https://github.com/serhatbolsu/robotframework-appiumlibrary
* **Note: This is w.r.t Python3**

## Set lambdatest Credentials 
* You can export the environment variables for the Username and Access Key of your lambdatest account. 

  ```
  export LT_USERNAME=<lambdatest-username> &&
  export LT_ACCESS_KEY=<lambdatest-access-key>
  ```

## Running tests

### App Automate

* Navigate to `cd app/test`
* Upload app refer https://www.lambdatest.com/support/docs/running-appium-tests-with-python/ or go to this link https://applive.lambdatest.com/app and upload your test then click on the 3 dots and then copy app id.
* Sample app:  your sample test path is app/test/WikipediaSample.apk
* Replace "app_url" from script with the response recieved while uploading your test app to Lambdatest . Eg: lt://APP10020521642428466273345 ( or the copied app id)
- Android
```

* Parallel Execution: 
* To run parallel tests, navigate to 'parallel' folder, run `cd parallel`
  1. Test Suite level
    - Run `pabot --processes <count_of_parallels> *.robot`
    - Alternate method: `pabot --processes <count_of_parallels> <name_of_suites_to_run>` Eg: `pabot --processes 2 Suite1_App.robot       Suite2_App.robot`
check your tests on lambdatest dashboard.
    

  

