## Section 3: Advanced Debugging Features

Advanced Debugging Features

# What I Learned

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
    - Note break point is frozen here

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

<hr>

- Arithmetic exception is occurring we can break on it in debugger

- Division by zero is going to **occur** here

<img src="exceptionAboutArithemamitcIsHolded.JPG" alt="alt text" width="500"/>


<img src="arithemitcException occurred.JPG" alt="alt text" width="500"/>

- **Exception breakpoint** stops programs when exception is happened

<img src="exception BreakPoint.jpg" alt="alt text" width="500"/>

1. You can add exception breakpoint using this button.
    - This particularly exception is occurring 

<img src="arithemitcExceptionSelectedJPG.JPG" alt="alt text" width="500"/>

<br>

<img src="exceptionGetCaugh.jpg" alt="alt text" width="500"/>

- If we put general `Exception` all other sub exceptions would be caught and modify it as following. **Subclasses of this exception**

<img src="andThis.JPG" alt="alt text" width="500"/>

- **Method Breakpoint** You can put breakpoint on method

<img src="methodBreakPoint.JPG" alt="alt text" width="600"/>

1. You can specify when break is occurring entering to function or when leaving function

<img src="callStackOfFramesInRecursingMethods.JPG" alt="alt text" width="600"/>

- Recursion function is taking place 

1. We can see call stack with frames

<img src="dropToFrame.JPG" alt="alt text" width="600"/>

1. **Drop To Frame** kinda "rewinds" the application to the state which was **Dropped to Frame**

- **Todo** Tee joku Proto projeti jossa käy ilmi tämä

- [Debug View](https://help.eclipse.org/latest/index.jsp?topic=%2Forg.eclipse.jdt.doc.user%2Freference%2Fviews%2Fdebug%2Fref-droptoframe.htm)
- [Drop Frame](https://help.eclipse.org/latest/index.jsp?topic=%2Forg.eclipse.jdt.doc.user%2Freference%2Fviews%2Fdebug%2Fref-droptoframe.html)

- Todo asenna ja suorita tomcatilla