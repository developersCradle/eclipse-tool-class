## Section 2: Basic Debugging Features

 Introduction to Java Debugging Using Eclipse

# What I Learned

- Debugging is a methodical process of finding and fixing the bugs in software.

<br>

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

### **Step into selection**

<img src="StepIntoSelection.JPG" alt="alt text" width="500"/>

- If you want to go into code inside some chained methods
    - Example `int firstPersonAge = DataUtil.getPersonData().get(0).getAge();`. We would want to go inside `getAge()` whiteout putting breakpoint manually

1. We first focus on method where want to go → Right click and select **Step Into Selection(CTRL+F5)**

- We will find end in `getAge()`

<img src="breakAfterStepInto.JPG" alt="alt text" width="500"/>

- We can ignore other breakpoints and run into specific line using

<img src="runIntoLine.JPG" alt="alt text" width="500"/>

- Skip all breakpoints. **Easy to leave on!**

<img src="skipAllBreakPoint.JPG" alt="alt text" width="700"/>

- We can evaluate expressions from `Highlight Expression` then click `Inspect`

<img src="InspectExpressions.JPG" alt="alt text" width="400"/>

- We can watch expression getting folded out
    - This can be also done in ahead in executed time

<img src="InspectExpressionsResults.JPG" alt="alt text" width="300"/>

<br>

- Execute can evaluate input ahead of time, just like inspect expression

<img src="Execute.JPG" alt="alt text" width="600"/>

<br>

<img src="expressions.JPG" alt="alt text" width="400"/>

- Expressions are also good way to evaluate values at execution time.
