## Informal Meeting Minutes of Software Engineering Group Project (1)

****

### 1. Basic Information

* Date: 15/10/2020
* Starting time: 13:00
* Ending time: 14:30
* Attendees: 
  * [Enze REN](../../CV/EnzeRen.md) (20127138)
  * [Chuyan FU](../../CV/ChuyanFu.md) (20124842)
  * [Chenyu YANG](../../CV/ChenyuYang.md) (20125098)
  * [Kailiang NAN](../../CV/KailiangNan.md) (20125247)
  * [Jiahe LYU](../../CV/JiaheLyu.md) (20125872)
  * [Chen SHAN](../../CV/ChenShan.md) (20126659)
* Absentees and reasons: N/A
* Recorder: Kailiang Nan (20125247)

### 2. Brief workflow

* List the basic functionalities of MIPS datapath Simulator
* discuss technical details of this project
* Discuss prerequisite knowledge we should learn
* Decide the first step of this project is to collect requirements from MIPS module conveners as well as Y3 students, to draw User case diagram, Sequence Diagram, Class Diagram.
* allot tasks to each members
* Decide the deadline of Requirement Analysis and UML design is **2020/10/18**, the deadline of Specification is **2020/10/20** 
* Discuss how to build the website. The details of website will be discussed in **2020/10/20**

### 3. Note of this meeting

#### Analyze basic functions of MIPS Datapath Simulator 

##### Code and output Module

1. Provide Code highlight

   * details

   * Different types of Instructions should be rendered in different color.

     * The animation is played according to each atomic instruction. I. e., the animation Simulate the datapath of only one instruction. So the line of instruction being animated will also be highlight.  

   * Possible Solution(Technical details)
     * Codemirror(A Javascript component)
     * writing this functionality in CSS and javascript on our own. 

2. Code line jumping(optional)

   * details
     * give users an input box to decide which line they want to jump to 
   * Possible Solution(Technical details)
     * javascript

3. Code reset button

   * details
     * A button for cleaning up all the code
   * Possible Solution(Technical details)
     * javascript

4. Code upload and download

   * details
     * Allow user to import and export their code from this software
   * Possible Solution(Technical details)
     * Unknow. No one know exactly how to fulfill this.

5. Log in and save Code(optional)

   * details

     * Allow user to login with their university account and access their history code.

   * Possible Solution(Technical details)

     * Contact with ITServices, use the login API of University.

     * cookies
     * database

6. Code Analysis(Syntax Analysis)

   * details
     * Our project should have the ability to figure out whether the code is correct
     * prompt the line that have incorrect code
     * show the specific details of the error
   * Possible Solution(Technical details)
     * javascript
     * Ajex

7. Code

   * details
     * put your cursor at a certain instruction, the corresponding component such as ALU or  Memory in the visualization Module will be highlight
   * Possible Solution(Technical details)
     * CSS and javascript
     * Code Module and Visualization Module can interact with each other using ????(unknown)

8. Output block

   * details
     * the output of executing code can be seen in the block
   * Possible Solution(Technical details)
     * CSS and javascript

##### Visualization module

1. Visualization of Register

   * details
     * When users double click the image of visualized register component. A block of window will pop up showing the visualized image of all registers
     * Users can modify values in registers
   * Possible Solution(Technical details)
     * CSS + SVG + javascript
     * OpenGL/WebGL

2. Visualization of Memory

   * details
     * When users double click the image of visualized memory component. A block of window will pop up showing all units of memory.
     * Users can modify values stored in registers
   * Possible Solution(Technical details)
     * CSS + SVG + javascript + HTML
     * OpenGL/WebGL

3. Visualization of  running Code

   * details

     * when the code is loaded into visualization parts. All the components in the visualization module will interact with each other to show the dataflow of all the instructions in the code.

     * The data will be spheres marked with their values

     * The components that is associated with executing current instruction will be highlighted.

     * When users stop playing the animation, they can put their cursor on a specific component to see what work it has done in the previous instruction. All the bus and components which interact with this component will be rendered in a different color.

       ![1](/markdown_image/sample1.png)

       >  image above shows the rough idea of the final effect of this function 

   * Possible Solution(Technical details)

     * CSS + SVG + javascript + unknown
     * OpenGL/WebGL

4. Control of Visualized animation

   * details
     * Execute one instruction at a time: Execute the previous instruction. Execute the next instruction. Execute from the start.
     * Execute all the instructions in the code at a time
     * Control the playing speed of animation
   * Possible Solution(Technical details)
     * CSS + SVG + javascript + unknown
     * OpenGL/WebGL

##### Guide Module

1. When a component in visualized module is chosen, the brief explanation of this component will popup.
   * detail
     * pending
   * Possible Solution(Technical details)
     * Unknown
2. The guide of the whole website
   * detail
     * pending
   * Possible Solution(Technical details)
     * Unknown
3. A button for importing a demo of how to use this websites
   * detail
     * An assembly code demo which can print "Hello world" on the screen will be given. Users can click the button to import this demo and the website will automatically play the animation.  
   * Possible Solution(Technical details)
     * Unknown

##### optional functionalities

1. The inverse operation: Users operates components in the visualization module and input the value in memory and registers. They choose how the data flow and how ALU works. A button will be given for them to generate code according to operations
   * Translate into Chinese: 代码逆向，操作图像部件生成代码
2. Assemble of circuit. This may give students a more impressive experience. Thus, enhance their understanding of how MIPS instructions work.
   * Translate into Chinese: 电路拼装，加强教学

#### Start of our project: the first step

##### Requirement Gathering

1. Contact module conveners of MIPS: [**Heng Yu**](https://www.nottingham.edu.cn/en/Science-Engineering/People/Profile.aspx?id=11d4b32a-2328-417a-b46d-9d82ac4cbeb5&language=en-GB) and [**Ying Weng**](https://www.nottingham.edu.cn/en/Science-Engineering/People/Profile.aspx?id=66f6267c-16fd-47d2-98cd-5e8b9c8bd894&language=en-GB). Ask the requirement of this project.
2. Collect survey from Y2 or Y3 students. option: Online collecting?
3. This task is appointed to **Kailiang Nan**(Contact [**Heng Yu**](https://www.nottingham.edu.cn/en/Science-Engineering/People/Profile.aspx?id=11d4b32a-2328-417a-b46d-9d82ac4cbeb5&language=en-GB), write Requirement), **Enze Ren**(Contact [**Ying Weng**](https://www.nottingham.edu.cn/en/Science-Engineering/People/Profile.aspx?id=66f6267c-16fd-47d2-98cd-5e8b9c8bd894&language=en-GB), write requirement) 

##### Draw UML diagrams

1. User Case Diagram(**Jiahe LYU**)
2. Class Diagram(**Chen Shan** and **Chuyan Fu**)
3. Sequence Diagram(**Chenyu yang**)

### prerequisite knowledge

1. MIPS
2. CSS,HTML,javascript,SVG
3. OpenGL(optional)

### website set up

1. advice: use bootstrap framework or modify from **Jiahe LYU**'s last semester's CW. 
