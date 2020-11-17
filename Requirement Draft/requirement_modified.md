### Requirement Analysis in text

​	The project is proposed by Ruibin Bai who was once the module convener of System and Architecture. The aim of this software is to aid students in learning how hardware responds to MIPS instructions. The basic requirements are listed as follows:

> 1. The simulator takes a fragment of MIPS program and simulate the flow of data components in different units of an MIPS CPU. The simulator should support the following type of 32-bit instructions:
>
>    1) I-type 
>
>    2) R-type 
>
>    3) J-type
>
> 2. The simulator will be used by UNNC qualifying year students as part of the lab tools to assist them in learning MIPS programming. The system should allow the users to debug and execute a given simple MIPS fragment and visualize the data flow between different MIPS CPU components.
>
> 3.  A web-based MIPS datapath simulator that can be deployed on CSLinux.

Target user: qualifying year student(sophomore)

Basic functionalities:

1. simulate the flow of data
2. support 3 types of 32-bits instructions
3. allow users to debug and execute MIPS code
4. Finally the project can be deployed in CSlinux

  Apart from the basic requirements, our developing team brought up more detailed requirements.

* The simulator consists of two modes, namely single-instruction mode and pipeline mode. The user can switch the mode according to  his need.
* The simulator should allow the students to input their code in the code block and different parts of the instruction should be rendered into different colors. For example, the operator, the operand and variable should be in different colors.
* The simulator should point out the mistakes in users' code. A error message should be given, specifying which part of the code goes wrong. This helps the users to debug.
* The output and running information will be displayed in the output block after each instruction being executed.
* The user is allowed to clean up all the running information and re-initialize the whole software.
* When the user double clicks the image of the visualized register component, a block of window will pop up showing the visualized image of all registers in detail and the user can edit the values of the registers if he wishes.
* When the user double clicks the image of the visualized memory component, a block of window will pop up showing all units of memory in detail and the user can edit the value of the memory for a specific address if he wishes.
* The flow of the data should be visualized.
* When the user stops playing the animation, they can put their cursor on a specific component to see what binary data is stored in this component.
* When the simulator is in the single-instruction mode, the user can switch between five different stages, namely IF, ID, EX, MEM and WB. The user can click on one of the five buttons to see the components that is being used in a specific stage. 
* An assembly code demo which can print "Hello world" on the screen will be given. The user can click the button to import this demo and the website will automatically play the animation.  
* When the cursor hovers over a visualized component, the brief explanation of this component will popup.

Some technical requirement

1. Module separation: Divided the whole project into four modules
   * Code input module
   * Visualization module
   * Control module
   * Console module
2. A good command of MIPS programming is required.
3. Skills about CSS, HTML, Javascript, typescript and SVG are needed.


