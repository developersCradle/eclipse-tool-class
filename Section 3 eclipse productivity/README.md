## Section 3: Managing Source Code

 Managing Source Code

# What I Learned


### Open Type

- Open class by name

<img src="openType.JPG" alt="alt text" width="500"/>

- We can open type by name from here

<img src="YouCanUseWildCardsAlso.JPG" alt="alt text" width="500"/>

- You can use **wildcards** in Eclipse. Here is usage when opening type

<img src="YouCanUseWildCardsAlso.JPG" alt="alt text" width="500"/>

### Quick Outline

- You can open outline view

<img src="quickOutlineOppening.JPG" alt="alt text" width="400"/>

- And it will look like such

<img src="quiqk outline.JPG" alt="alt text" width="500"/>

- You can also filter in this menu

### Display inheritance tree

> **Navigate** > **Open Type Hierarchy** 

- This will help you to look inheritance tree for class

<img src="typeHierachy.jpg" alt="alt text" width="600"/>

### Display Quick Inheritance Tree

> Right-click > Quick Type Hierarchy

<img src="quickTypeHierachy.jpg" alt="alt text" width="500"/>

- Quick Type Hierarchy

1. You can type to filter 

### Search For Text

> CTRL + F

- Search for text, with different tools

<img src="searchText.jpg" alt="alt text" width="600"/>

- If you have multiple files

### Search For Multiple Files

> Search > Search 

<img src="searchFiles.jpg" alt="alt text" width="600"/>

1. **File Search**, can search plain text from multiple files
2. **Git Search**, you can search against Git repository
3. **Java Search**, search against Java constructs

<img src="typeSearch.jpg" alt="alt text" width="600"/>

1. We are searching for where `JButton` is used in this project

<img src="searchMethod.jpg" alt="alt text" width="600"/>

1. We are using `*` wild card with method name `create*`. Searching **method** name start with `create`

### View Method Detail

> Right-click > Open Declaration (**F3**)

- Opens declaration of method when opened 

### Finding Reference For Method

> Right-click > References > Workspace

<img src="findingReferencesInWorkspace.jpg" alt="alt text" width="600"/>

- We can look where this method is being called

### Call Hierarchy: Sequence of methods calls

> Right-click > Open Call Hierarchy

- Given sequence of methods calls

<img src="callHierachyCalls.jpg" alt="alt text" width="600"/>

1. We are calling `Call Hierachy` here
2. We are reading this from **top** to **bottom**. **Main method** is calling our **constructor** which in sense is calling **our method** `create*` 

### Generating Getters and Setters

> Right-click > Source > Generating Getters and Setters

<img src="generartingGettersAndSetters.jpg" alt="alt text" width="600"/>

1. We can generate fetters and setters from class fields

### Generating Constructor using fields

> Right-click > Source > Generating Constructors using fields

<img src="generartingConstructorUsingFields.jpg" alt="alt text" width="500"/>

### Override / Implement Methods

> Right-click > Source > Override / Implement Methods

<img src="override.jpg" alt="alt text" width="500"/>

- Usually we be overriding `toString()` method

### Template shortcuts

<img src="ctrl+space.jpg" alt="alt text" width="500"/>

1. `Ctrl+Space` will auto complete code from template 
    - These can be found in Eclipse 
> Java > Editor > Templates > Main

<img src="templateList.jpg" alt="alt text" width="500"/>

### Format

> Right-click > Source > Format


### Refactoring

<img src="refactoring.png" alt="alt text" width="400"/>

### Extract Constant

<img src="exctractConstant.png" alt="alt text" width="400"/>

1. Write new for **Extracted Constant**

<img src="exctractConstantt.jpg" alt="alt text" width="400"/>

1. Extracted to own variable

### Extract Local Variables

> Color the code which you want to extract from code > Refactor > 

**Extract Local Variable**

### Extract Methods

<img src="excractMethod.jpg" alt="alt text" width="400"/>

1. We can see this is one logical chunk of code, we want to extract this one

> Color the code which you want to extract to method > Refactor > **Extract Method...**

- Input name here to be refactored into 

<img src="nameForExctractedMethod.jpg" alt="alt text" width="400"/>

### Rename Method or variable

- Renaming method or variables

> Right-Click > Refactor > Rename...
