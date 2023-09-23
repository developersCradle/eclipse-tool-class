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

<img src="expressions.JPG" alt="alt text" width="400"/>

<br>

- We can look differently created object. **Show logical structure** or whiteout 

<img src="showLogicalStructures.JPG" alt="alt text" width="400"/>

1. We can toggle this and remove this from button.

<img src="whitoutLogicalStucture.JPG" alt="alt text" width="400"/>

- Whiteout there a lot of "extra" methods. Like form arrays methods

<br>

<img src="debugShell.JPG" alt="alt text" width="400"/>

<br>

<img src="debugShell1.JPG" alt="alt text" width="400"/>

<br>

1. You can execute piece of code here even if debug console is frozen in certain line. In example, **evaluate size of personData()**. Using button **Display Result of Evaluating Selected Text** 

2. You can see evaluated value returned from expression

3. Executes without returning value 

<img src="debugShell1console.JPG" alt="alt text" width="300"/>

<br>

<img src="debugSessionToString().JPG" alt="alt text" width="500"/>

1. Eclipse normally outputs **Object** to using `toString()` to debug window
    - Note bp is frozen here

- We can change formatting in eclipse

<br>

<img src="weCanCreateFormatter.JPG" alt="alt text" width="500"/>

- We can create debug formatter here

- We will write formatter for `Person.java` class
    - We just describe the output format

<img src="configuringDebugFormatter.JPG" alt="alt text" width="500"/>

<br>

<img src="debugFormatterWorking.JPG" alt="alt text" width="500"/>

1. We can see the configured formatter working

- We can debug **specific** object in **List**. Furthermore, we can achieve this using **conditional breakpoint**

<img src="conditionalBreakPoint.JPG" alt="alt text" width="500"/>

<br>

1.  We can modify breakpoint from **Breakpoint Properties...**

<img src="conditionalBreakPointConfiguring.JPG" alt="alt text" width="500"/>

- We put **`ON`** Conditional

1. Place **logic** for triggering **breakpoint** 
    - This one will be breaking when country is **`US`**

<img src="brakePointOccurredUS.JPG" alt="alt text" width="500"/>

<br>

- As you can see program has halted in **`US`** Element

<img src="iterationHitCountBp.JPG" alt="alt text" width="500"/>

<br>

1. You brake on hit count example here is specified 6 hit count
2. You can see 5 `println` occurred and 6 has been halted

<img src="howToDebugExpection.JPG" alt="alt text" width="500"/>
