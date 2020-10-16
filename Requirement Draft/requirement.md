### Requirement Analysis in text

​	The project is proposed by Ruibin Bai who was once the module convener of System and Architecture. The aim of this software is to aid students learning how hardware respond to MIPS instructions. The basic requirement is listed as follow:

> 1. The simulator takes a fragment of MIPS program and simulate the flow of data components in different units of an MIPS CPU. Your simulator should support the following type of 32-bit instructions:
>
>    1) I-type 
>
>    2) R-type 
>
>    3) J-type
>
> 2. The simulator will be used by UNNC qualifying year students as part of lab tools to assist them learning MIPS programming. The system should allow users to debug and execute a given simple MIPS fragment and visualize the data flow between different MIPS CPU components.
>
> 3.  A web-based MIPS datapath simulator that can be deployed on CSLinux。

Target user: qualifying year student(sophomore)

Basic functionalities:

1. simulate the flow of data
2. support 3 types of 32-bits instructions
3. allow users to debug and execute MIPS code
4. Finally the project can be deployed in CSlinux

  Apart from the basic requirements, our developing team brought up more detailed requirements.

* The simulator should allow students to input their code in the code block and instructions of different types should be rendered into different colors.
* The simulator should point out the mistakes in users' code. Underlining where the code goes wrong.(help debug)
* The output and running information will be displayed in the output block after each instruction being executed.
* Allow user to clean up all the running information. Re-initialize the whole software.
* When users double click the image of visualized register component. A block of window will pop up showing the visualized image of all registers
* When users double click the image of visualized memory component. A block of window will pop up showing all units of memory.
* When users stop playing the visualized animation, they can put their cursor on a specific component to see what work it has done in the previous instruction. All the bus and components which interact with this component will be rendered in a different color.
* An assembly code demo which can print "Hello world" on the screen will be given. Users can click the button to import this demo and the website will automatically play the animation.  
* The simulator will provide users basic usages. The user can turn on/off the tutorial/guidance by themselves.
* When a component in visualized module is chosen, the brief explanation of this component will popup.
* The users can set their coding preference in the control module. Some basic functions include change the font size, turn on or turn off functions

Some technical requirement

1. Module separation: Divided the whole project into three module
   * Code and output module
   * Visualization module
   * Guide module
   * Control module
2. As a developer you should first have a good command of MIPS programming.
3. CSS,HTML,Javascript,SVG is needed.

Kailiang Nan