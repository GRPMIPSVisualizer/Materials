## Specification - Tabular

### 1. Component visualization area

| Function                        | Description                                                  | The corresponding prototype |
| ------------------------------- | ------------------------------------------------------------ | --------------------------- |
| Visualization of Register       | The simulator will show a block of window which has the visualized image of all registers, when users double click the image of visualized Register component. And then users can click the text box and input the value of the data as they want. The simulator wil show a block of window which has the visualized image of all instruction registers, when users double click the image of visualized Instruction register component. And then users can click the text box and input the value of the instruction data as they want. | 1.7                         |
| Visualization of Memory         | The simulator will show a block of window which has all units of memory, when users double click the image of visualized Memory component. And then users can click the text box and input the value of the stored value in registers as they want. | 1.7                         |
| Visualization of running Code   | When the code is loaded, the simulator will highlight the components which are associated with the current instruction. And then the sphere with whe values will move from the start point. As the ball passes through the register, the corresponding register changes. Finally the sphere will go through the all instructions and the simulator will stop. | 1.7                         |
| Control of Visualized animation | When the button 'step backward' is clicked, the simulator will show the stage that is backward the current stage and the sphere will move to the previous position. When the button 'step forward' is clicked, the simulator will show the stage that is forward the current stage and the sphere will move to the next position. When the button 'pause' is clicked, the simulator will stop the execute and the sphere will also stop moving. When the button 'run' is clicked, the simulator will execute until the end and the sphere will continue its moving. When the button '0.5x' is clicked, the simulator will run the instruction in the half speed, it will become slowlier than normal state. When the button '2.0x' is clicked, the simulator will run the instruction in the twice speed, it will become faster than normal state. When the button 'IF', 'ID', 'EX', 'MEM' or 'WB' is clicked, the simulator will display the animation of the corresponding CPU stage. | 1.6; 2.2 |
| Visualization of binary code | When a user click on a specific component which holds binary code inside it, the page should be able to not only show the description of the component but also the binary codes in it. | 2.3 |
### 2. Debug area

| Function                          | Description                                                  | The corresponding prototype |
| --------------------------------- | ------------------------------------------------------------ | --------------------------- |
| Inform users of running condition | The web page shall be to inform users when following situations occured: the program has been compiled and run successfully; the code failed to compile; the speed of running has been changed; the animation switched to last/next instruction; the code has been upload/download successfully. | No 1.6                      |
| Inform users of compiling error   | The web page shall be able to inform users about the lines that have syntax error and reasons for them. | No. 1.5                     |

### 3. Code writing area

| Function                           | Description                                                  | The corresponding prototype |
| ---------------------------------- | ------------------------------------------------------------ | --------------------------- |
| Code highlight                     | The system shall be able to provide code highlight according to different code type. Comments shall be green, registers shall be red, instructions shall be blue, Code segmentation flags shall be pink and others shall be black. | No. 1.1                     |
| Code highlight while running       | The animation simulates the datapath of only one instruction, so the line of instruction being animated shall also be highlighted by the web page. | No. 1.6                     |
| Page reset                         | The web page shall be able to reset the code area, animation area and the debug area at the same time by clicking the reset button. | No. 1.11                    |
| Compile and run the code           | The web page shall be able to compille and run the code while user click the 'run' button | No. 1.6                     |
| Upload code file from local device | The web page shall be able to allow users to upload asm files from their local device by clicking the 'upload' button. | No. 1.3                     |
| Download code to local device      | The web page shall be able to allow users to download the code in the coding area to their local device by clicking the 'download' button. | No. 1.4                     |

### 4. Navigation bar

| Function                                                | Description                                                  | The corresponding prototype |
| ------------------------------------------------------- | ------------------------------------------------------------ | --------------------------- |
| Get help                                                | The page should automatically go to a new page with the specific User Manual when the user clicks the 'Help' button. | 1.9                         |
| Run demo code                                           | A piece of 'Helloworld' code should automatically load in the code input area on the right side of the web page after the user clicks the 'Demo' button. This code runs after the user clicks the Run button and prints 'hello world' in the Debug area. | 1.10                        |
| Mode switching | The web page should be able to allow users switch between single-instruction tutorial mode and the advanced pipeline mode, by clicking the 'mode' button in the navigation bar. | 2.1 |
