# COS 132 - Imperative Programming

## Algorithmic Thinking
$\Rightarrow$ __Decomposition__: Breaking the problem into smaller parts.  
$\Rightarrow$ __Pattern Recognition__: Identifying similar parts previouslt defined or from experience.  
$\Rightarrow$ __Abstraction__: Identifying the steps required to solve the problem.  
$\Rightarrow$ __Algorithm__: Formalising the final algorithm from the abstracted steps.  

## Flowcharts
### Elements
| Symbol | Description | Illustration |
| -- | -- | -- |
| Start | The start symbol indicates where the initial/entry point is for the algorithm represented by the flowchart. | ![Start Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/Start.png) |
| End | The end symbol indicates the termination point of an algorithm represented by the flowchart. | ![End Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/End.png) |
| Process | The process symbol is used to indicate operations or maniplation of data is performed at that stage of the algorithm. | ![Process Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/Process.png) |
| Process | The predefined process indicates a pre-defined sub-process that forms part of the algorithm but the steps are not explicitly shown or formalised yet. | ![Predefined Process Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/Predefined_Process.png) |
| Decision | The decision symbol indicates a choice/decision that is performed which can result in two or more alternative "paths" through the flowchart. The alternative options are labelled. | ![Descision Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/Decision.png) |
| Input/Output | This symbol is used to model input from external sources, like user input, or output to external sources like terminal output. | ![Input/Output Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/Input_Output.png) |
| Flow arrows | The flow arrow symbol is used to indicate the direction of the information flow. | ![Flow arrow Symbol](https://github.com/DiabGarren/COS-132_Imperative-Programming/blob/main/Flow_Arrow.png)

### Structures
- __Linear Execution__: A set of instructions that are executed in order one after the other to form a _sequential structure_.
- __Decision Making__: A point in the algorithm where two or more alternative options can be selected which form a _selection structure_.
- __Repetition__: A set of instructions which are repeated until some termination condition is satisfied to form _repetition structures_.

### Drawing
- Ensure that flowcharts are easy to read and easy to follow.
- Flowcharts should fit on a single page.
- The sizes of shaped should remain consistent.
- Ensure that the styling of the flow arrows remains consistent.
- The font and styling of the text used in the flowchart remain consistent.
- Ensure that, as far as possible, the flow arrows do not cross.
- Ensure that flow arrows consist of straight lines.
- Ensure symbols are appropriately spaced out.

## Logo
### General Structure
Logo statements are generally structured as:
```instrName <value1, value2, $\dots$, valueN>```  
### Turtle Statements
| Command | Short Form | Example | Description |
| -- | -- | -- | -- |
| FORWARD | FD | ```FD 100``` | Moves the turtle forward. (100 steps) |
| BACK | BK | ```BK 50``` | Moves the turtle back. (50 steps) |
| LEFT | LT | ```LT 90``` | Turns the turtle left. (90 deg) |
| RIGHT | RT | ```RT 45``` | Turns the turtle right. (45 deg) |
| PENUP | PU | ```PU``` | Stops the pen from drawing. |
| PENDOWN | PD | ```PD``` | Enables the pen to draw. |
| SETPENCOLOR | | ```SETPENCOLOR 0``` | Changes the pen colour. |
| SETBACKGROUND | SETBG | ```SETBG 7``` | Changes the background colour. | 
| CLEARSCREEN | CS | ```CS``` | Clears all pen markings from the screen, and moves the turtle to the origin. |
| SETPOS | | ```SETPOS [0 0]``` | Moves the turtle to the given coordinates. |
| SETX | | ```SETX 0``` | Moves the turtle to the given x coordinate. |
| SETY | | ```SETY 0``` | Moves the turtle to the given y coordinate. |
| SETHEADING | SETH | ```SETH 0``` | Changes the direction the turtle if facing. (0 - North, 180 - South) | 

### Turtle Pen Colours
| Value | Colour | Number | Colour | Name | Colour |
| -- | -- | -- | -- | -- | -- |
| 0 | $\color{black}{\text{Black}}$ | 6 | $\color{yellow}{\text{Yellow}}$ | 12 | $\color{salmon}{\text{Salmon}}$ |
| 1 | $\color{blue}{\text{Blue}}$ | 7 | $\color{white}{\text{White}}$ | 13 | $\color{purple}{\text{Purple}}$ |
| 2 | $\color{green}{\text{Green}}$ | 8 | $\color{brown}{\text{Brown}}$ | 14 | $\color{orange}{\text{Orange}}$ |
| 3 | $\color{cyan}{\text{Cyan}}$ | 9 | $\color{tan}{\text{Tan}}$ | 15 | $\color{grey}{\text{Grey}}$ |
| 4 | $\color{red}{\text{Red}}$ | 10 | $\color{#357446}{\text{Forest}}$ | | |
| 5 | $\color{magenta}{\text{Magenta}}$ | 11 | $\color{aqua}{\text{Aqua}}$ | | |

## C++ vs. Logo
### Variables
| C++ | Logo |
| -- | -- |
| ```int x = 5;``` | ```MAKE "x 5``` |
| ```char myChar = 'a';``` | ```MAKE "mychar "a``` |
| ```bool val = true;``` | ```MAKE "val "true``` |
| ```std::string str = "Hello World";``` | ```MAKE "str (SENTENCE "Hello "World)``` |
| ```int arr[5] = {};``` | ```MAKE "arr []``` |

### Output
| C++ | Logo |
| -- | -- |
| ```std::cout << x + y << std::endl;``` | ```PRINT (SUM :x :y)``` |
| ```std::cout << arr[1] << std::endl;``` | ```PRINT (ITEM 2 :arr)``` |
| ```std::cout << "Hello World! << std::endl;``` | ```PRINT (SENTENCE "Hello "World "!)``` |

### Input
| C++ | Logo |
| -- | -- |
| ```std::cin >> input;``` | ```MAKE "input READCHAR``` |
| ```std::getline(std::cin, input);``` | ```MAKE "input READWORD``` |

### Arithmetic Operations
| C++ | Logo |
| -- | -- |
| ```x + y``` |```SUM :x :y```|
| ```x - y``` |```DIFFERENCE :x :y```|
| ```x * y``` |```PRODUCT :x :y```|
| ```x / y``` |```QUOTIENT :x :y```|
| ```x % y``` |```MODULO :x :y```|

### Operands
| C++ | Logo |
| -- | -- |
| ```x == y``` | ```:x = :y``` |
| ```x != y``` | ```:x <> :y```|
| ```x > y``` | ```:x > :y```|
| ```x >= y``` | ```:x >= :y```|
| ```x < y``` | ```:x < :y```|
| ```x <= y``` | ```:x <= :y```|
| ```x && y``` | ```AND :x :y```|
| ```x && y && z``` | ```AND :x :y :z```|
| ```x \|\| y``` | ```OR :x :y``` |
| ```x \|\| y \|\| z``` | ```OR :x :y :z``` |
| ```!x``` | ```NOT :x``` |

### If Statements
| C++ | Logo |
| -- | -- |
| ```if (x == y ) {``` <br> ```}``` | ```IF (:x = :y) [``` <br> ```]``` |
| ```if (x != y ) {``` <br> ```} else {``` <br> ```}``` | ```IFELSE (:x <> :y) [``` <br> ```] [``` <br> ```]``` |

### Loops
| C++ | Logo |
| -- | -- |
| ```for (int i = 0; i < 10; i++) {``` <br> _```    // body of the loop```_ <br> ```}``` | ```REPEAT 10 [``` <br> _```    ; body of the loop```_ <br> ```]``` |
| ```while (x > 5) {``` <br> _```    // body of the loop```_ <br> ```}``` | ```WHILE [: > 5] [``` <br> _```    ; body of the loop```_ <br> ```]``` |
| ```do {``` <br> _```    // body of the loop```_ <br> ```} while (y < 10);``` | ```DO.WHILE [``` <br> _```    ; body of the loop```_ <br> ```] [:y < 10]``` |

### Functions
| C++ | Logo |
| -- | -- |
| ```void myFunc() {``` <br> ```}``` | ```TO myFunc``` <br> ```END```|
| ```int myFunc(int x, int y) {``` <br> ```    return x + y;``` <br> ```}``` | ```TO myFunc :x :y``` <br> ```    OUTPUT (SUM :x :y)``` <br> ```END```|
