## Section 2: Basic Debugging Features

 Introduction to Java Debugging Using Eclipse


# What I Learned

- Debugging is a methodical process of finding and fixing the bugs in software.
- Breakpoint is pause in code.

<br>

- **Step Over (F6)**, Line get executed and control is given in next line

<img src="stepOver.JPG" alt="alt text" width="500"/>

- **Step Into (F5)**
    - Steps into function/method
- **Step Return (F7)**
    - Function/method will be executed and control is returned to caller

<img src="stepReturn.JPG" alt="alt text" width="500"/>

<hr>

<img src="EclipseDebuggingTricks.JPG" alt="alt text" width="300"/>

#### Step into selection

<img src="StepIntoSelection.JPG" alt="alt text" width="500"/>

- If you want to go into code inside some chained methods
    - Example `int firstPersonAge = DataUtil.getPersonData().get(0).getAge();`. We would want to go inside `getAge()` whiteout putting breakpoint manually

1. We first focus on method where want to go → Right click and select **Step Into Selection(CTRL+F5)**

- We will find end in `getAge()`

<img src="breakAfterStepInto.JPG" alt="alt text" width="500"/>

- Jäin 7:50