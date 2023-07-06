# TCL Workshop: From Introduction to Advanced Scripting Techniques in Design and Synthesis

TCL scripting plays a crucial role in the field of VLSI design and verification, making it an indispensable tool for semiconductor engineers. VLSI projects involve complex tasks such as chip design, simulation, verification, and manufacturing, and TCL scripting provides an efficient and flexible way to automate these processes. With TCL, engineers can write scripts to automate design tasks, perform simulations, analyze data, and generate reports, significantly reducing the time and effort required for repetitive tasks. TCL also offers excellent integration capabilities, allowing seamless interaction with other EDA tools and languages. Moreover, TCL scripting provides a high level of control and customization, enabling engineers to create complex workflows and implement design methodologies specific to their requirements. Overall, TCL scripting empowers VLSI engineers to enhance productivity, streamline workflows, and accelerate the development and verification of advanced integrated circuits.

# Workshop Details & Agenda

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/97e1264e-31a7-4539-a21b-639e3dd31e13)

VLSI System Design Corp. Pvt. Ltd. had proposed this 5 days workshop entitled as "TCL Workshop: From Introduction to Advanced Scripting Techniques in Design and Synthesis
" from 5th July 2023 to 9the July 2023 with the guidance of Mr. Kunal Ghosh, Co-Founder, VSD Corp. Pvt. Ltd. and Ms. Geetima Kachari who had been working as the Teaching Assistant throughout the entire workshop. The agenda for the workshop is as follows :

Day 1 (5th July 2023) : Serving as the foundation, introduction to the core concepts and tasks of TCL. 

Days 2 & 3 (6th & 7th July 2023): Immersing in the art of variable creation and processing constraints. 

Day 4 (8th July 2023) : Introduction to Yosys synthesis tool, understanding memory module RTL descriptions, and mastering gate level netlist descriptions.

Day 5 (9th July 2023) : Quality of Results (QOR) generation, optimization to precise WNS and FEP analysis.

# Day-wise Workshop Progress

- [Day 1 5th July 2023](#Day-1-5th-July-2023)
- [Day 2 6th July 2023](#Day-2-6th-July-2023)
- [Day 3 7th July 2023](#Day-3-7th-July-2023)
- [Day 4 8th July 2023](#Day-4-8th-July-2023)
- [Day 5 9th July 2023](#Day-5-9th-July-2023)

# Day 1  5th July 2023

# Tasks of the Day :

    • Create & Execute the Bash Script
    • Invoke TCL Command by accepting command line arguments
    • Deal with issues to pass command line argument to TCL Script (Eg. No Argument, Multiple Arguments, Argument doesn't exist)

# Script of the Day :


    #!/bin/tcsh -f
    
    echo "\n\n\n\n\t\t\t\t\t\tSYNTHIA\n\n"
    
    echo "\t\tAn automation created by Akash Ambekar for the Synthesis using TCL Scripting"
    
    echo "\t\t\t\tDuring the 5-Days Workshop entiled as :"
    
    echo "\tTCL Workshop: From Introduction to Advanced Scripting Techniques in Design and Synthesis"
    
    echo "\t\t\torganized By: VLSI System Design Corp. Pvt. Ltd."
    
    echo
    
    echo 
    
    echo
    
    if ($#argv != 1) then
    
        echo "SYNTHIA Info: Please provide a proper the csv file" exit 1
        
    endif
    
    if (!-f $argv[1]) then
    
        echo "SYNTHIA Error: Cannot find csv file $argv[1] in Directory. Exiting the Flow..."
        
        exit 1
        
    else
    
        tclsh synthia.tcl $argv[1]
        
    endif

# Results : 

Case 1) Normal Command Line Argument Passing

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/b1be5101-3f8d-476d-8156-144e051716a4)

Case 2) No Command Line Argument

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/d22920ec-11b0-4335-99c2-320b56c3575d)

Case 3) Multiple Command Line Arguments

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/7f4373c8-3e55-4243-bc12-c193d8d39695)

Case 4) Command Line Argument Doesn't Exist

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/566fea5d-3cd7-4902-af2a-03e406768235)


# Day 2 6th July 2023

# Tasks of the Day :

    • Auto Variable Creation
    • Checking if provided directories exist at respective locations, display an error if not found.....
    • Convert the inputs into a format that can be passed to Yosys Synthesis Tool

# Results 

1) Passing Inputs Path from .csv file to the Scripts :

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/f6be436e-d4fa-4877-9be8-e9c02362d873)

2) Checking the directories for given input path exists at respective locations or not :

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/e26ff860-a5f2-431c-8b68-2a8d4a3271b8)

3) Display an Error if the directory is not found at given location :

![image](https://github.com/akash-ambekar/VSD-5-DAYS-TCL-SCRIPTING-WORKSHOP/assets/100372947/ad894d25-b412-4f3d-b09c-1cd070b1e5cd)

# Day 3 7th July 2023

# Day 4 8th July 2023

# Day 5 9th July 2023
