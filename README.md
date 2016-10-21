# Using the Logger

[Logger library documentation](https://github.com/SergiusTheBest/plog)

#### Installation

1. Download the 2017-preseason-logger project to your workspace. 
2. Open this file path: 
      ```bash
      "c/Users/YOUR_USERNAME/workspace/2017-preseason-logger/src"
      ```
3. Copy plog folder.
4. Navigate to the project you want to copy to:
      ```bash
      "c/Users/YOUR_USERNAME/workspace/YOUR_PROJECT/src"
      ```
5. Paste plog folder into the src folder.
6. After completing the above tasks open Eclipse and refresh your project.
7. Finished :)

#### Initialization 

1. At the top of your project, include plog/Log.h and sys/stat.h
2. Enter the following code: 

      ```c++
      plog::init(plog::debug, "FILE_PATH");
      ```
      
3. Dooone :)

#### Rules

- Minimize number of logs otherwise there will end up being a very large amount of them to go through. 
- Only make new logs to differentiate between major topics.

##### When to Log
You should only log when you are:
- Trying to debug.
- Printing out values of components.
- Anything you would normally send to the dashboard. 

#### Conventions

Simple statements.

Include what data you are logging.

Example using 2016 robot code :

  ```c++
  PLOGD << "State: " << getCurrentState(); 
  ```
