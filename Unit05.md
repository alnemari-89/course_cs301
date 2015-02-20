---
layout: default
title: "CS301: Computer Architecture"
course_description: "An exploration of the basic hardware/software components, assembly language, and functional architecture design of computers."
next: ../Unit06
previous: ../Unit04
---
**Unit 5: Designing a Processor** <span id="5"></span> 
*In this unit, we will discuss various components of MIPS processor
architecture and then take a subset of MIPS instructions to create a
simplified processor in order to better understand the steps in
processor design. This unit will ask you to apply the information you
learned in units 2, 3, and 4 to create a simple processor architecture.
We will also discuss a technique known as* *pipelining, which is used to
improve processor performance. We will also identify the issues that
limit the performance gains that can be achieved from it. *  
  
 *In previous units, you learned about how computer memory stores
information, in particular how numbers are represented in a computer
memory word (typically, 32 or 64 bits); hardware elements that perform
logic functions; the use of these elements to design larger hardware
components that perform arithmetic computations, in particular addition
and multiplication; and the use of these larger components to design
additional components that perform subtraction and division. You also
looked at machine language and assembly language instructions that
provide control to hardware components in carrying out computations. In
this unit, you will learn about how the larger components are used in
designing a computer system.*

**Unit 5 Time Advisory**  
Completing this unit should take approximately 11.5 hours.  
  
 ☐    Subunit 5.1: 1 hour  
  
 ☐    Subunit 5.2: 1.25 hours  
  
 ☐    Subunit 5.3: 1.25 hours  
  
 ☐    Subunit 5.4: 1.25 hours  
  
 ☐    Subunit 5.5: 2 hours  
  
 ☐    Subunit 5.6: 1.25 hours  
  
 ☐    Subunit 5.7: 0.5 hours  
  
 ☐    Unit 5 Assessment: 3 hours

**Unit5 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   describe sequential or Von Neumann computer architecture;  
      
-   identify the hardware components used to develop the architecture of
    a processor;  
      
-   summarize the design of a simple MIPS processor;  
      
-   identify the factors that affect and limit the performance of a
    processor and its architecture; and  
      
-   describe the approaches used to improve process performance.

**5.1 Von Neumann Architecture** <span id="5.1"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 1: Sequential
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 1: Sequential
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Study section 1.1 of Chapter 1 on pages 7–13 to learn
    about sequential or Von Neumann computer architecture. Computer
    architecture is the high level computer design comprising components
    which perform the functions of data storage, computations, data
    transfer, and control. This reading also covers the topic outlined
    in subunit 5.5.  
        
     Studying this section and taking notes should take approximately 1
    hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**5.2 Simple MIPS Processor Components** <span id="5.2"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Processor Design: An Introduction”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Processor Design: An
    Introduction”](http://www.youtube.com/watch?v=0B-y1RPDXjs)
    (YouTube)  
        
     Instructions: Watch this lecture, which introduces the components
    of MIPS architecture that are required to process a subset of MIPS
    instructions. This is the first lecture of a series of video
    lectures on the design of a MIPS processor. This series of six
    videos incrementally design a processor that implements a subset of
    eight MIPS instructions: five arithmetic instructions, two memory
    reference instructions, and one flow control instruction. Using
    hardware components, referred to as building blocks, and a
    microprogram control, the lecturer executes these eight instructions
    to develop a simple design of a processor.  
        
     In this lecture, Kumar discusses the performance of the design and
    performance improvement using a multi-cycle design. Also, Kumar
    identifies an extension of the design to deal with exceptional cases
    that could occur when executing programs written using the eight
    instructions (exception handling). Lastly, the lecturer identifies
    increments to the design to include additional instructions.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1.25 hours.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**5.3 Designing a Datapath for a Simple Processor** <span
id="5.3"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Processor Design: Datapath”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Processor Design:
    Datapath”](http://www.youtube.com/watch?v=Ngu1UbRAeqQ&feature=relmfu) (YouTube)  
      
     Instructions: Watch this lecture, which is the second video in a
    series of six video lectures on the design of a MIPS processor. The
    previous video lecture presented the processor building blocks that
    will be used in the series. This video lecture explains how to build
    a datapath of the MIPS architecture to process a subset of the MIPS
    instructions. We will take R-format instructions and memory
    instructions and look into the datapath requirements to process
    them. Then, the other instructions will be addressed one at a time,
    and incremental changes to the design will be made to handle them.
    The data path and controller will be interconnected, and the (micro)
    control signals to perform the correct hardware operations at the
    right time will be identified. The next video in subunit 5.4 will
    look at the design of the controller.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1.25 hours.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**5.4 Alternative Approach to Datapath Design and Design of a Control
for a Simple Processor** <span id="5.4"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Processor Design: Control”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Processor Design:
    Control”](http://www.youtube.com/watch?v=kW_OuCEq_Iw&feature=relmfu) (YouTube)  
        
     Instructions: Watch this lecture, which is the third video of the
    series of video lectures on the design of a simple processor. This
    lecture explains how to build the control part of the MIPS
    architecture that is required to process a subset of MIPS
    instructions. This builds on the datapath design from the last
    lecture. That datapath design approach started with a design for the
    R class instructions – instructions having operands in registers,
    e.g., add, subtract, ‘and’, ‘or’, ‘less than’. It then included the
    other instructions, one at a time, and incremented the design to
    accommodate them. In this video lecture, an alternative approach is
    used to arrive at the same design. Here, the datapath for the
    arithmetic and logic instructions is designed. Then, the data path
    for the store, then for the load, then the branch on equal, and,
    finally, the jump are designed individually. Next, datapath design
    for all eight instructions is the union of the five individual
    designs. The control signals for each instruction are identified and
    combined to form a truth table for a controller, which is
    implemented using a PLA (program logic array). The video concludes
    with a performance/delay analysis of the design to show the
    limitations of a single cycle datapath. The next video in subunit
    5.5 will look at pipelining for increased performance.  
      
     Watching this lecture and pausing to take notes should take
    approximately 1.25 hours.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**5.5 Pipelining and Hazards** <span id="5.5"></span> 
*The reading assigned below subunit 5.1 covers this topic. Review
sections 1.1.1.1 Pipelining, 1.1.1.2 Peak Performance, 1.1.1.3
Pipelining beyond Arithmetic: Instruction Level Parallelism, and 1.1.1.4
8-bit, 16-bit, 32-bit, 64-bit, on pages 10–14.* *Take approximately 30
minutes to review this material.*

-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Pipelined Processor Design”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Pipelined Processor
    Design”](http://www.youtube.com/watch?v=pIBwr7Rx-1M) (YouTube)  
        
     Instructions: Watch this lecture, which presents basic ideas on
    improving processor performance through the use of pipelining. The
    previous video showed the limitations of a single cycle datapath
    design. To overcome the limitations and improve performance, a
    pipeline datapath design is considered. This video lecture explains
    pipelining. A pipeline datapathis analogous to an assembly line in
    manufacturing. First, you develop a skeleton design of a pipeline
    datapath. Performance analysis shows that several types of delays
    can arise, called hazards: structure, data, or control hazards.
    Design can address those arising from structure. However, data and
    control delays cannot always be prevented. The next video lecture
    will complete the design of a pipeline datapath for the simple
    processor.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1 hour and 30 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**5.6 Pipelined Processor** <span id="5.6"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Pipelined Processor Design: Datapath”**
    Link:  YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s [“Pipelined Processor Design:
    Datapath”](http://www.youtube.com/watch?v=SL_djmTegqc&feature=relmfu)
    (YouTube)  
      
     Instructions: Watch this lecture, which explains how to design a
    pipelined MIPS processor. The previous video introduced pipelining
    as a way to increase performance. It showed how hazards can limit
    the performance improvement of a pipeline datapath. This video
    lecture completes the design of a pipeline datapath. Ignoring
    hazards, the lecturer designs a control for the pipeline, integrates
    all the components including the control with the pipeline, and then
    considers the behavior with respect to hazards.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1.25 hours.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**5.7 Instruction Level Parallelism** <span id="5.7"></span> 
-   **Reading: Connexions: Charles Severance and Kevin Dowd’s
    “Understanding Parallelism – Introduction”**
    Link: Connexions: Charles Severance and Kevin Dowd’s [“Understanding
    Parallelism –
    Introduction”](http://www.saylor.org/site/wp-content/uploads/2014/01/CS301-5.7-UnderstandingParallelism-Introduction-CCBY.pdf) (PDF)  
      
     Instructions: Read this article, which discusses granularity of
    parallelism. On a uniprocessor, instruction level parallelism
    includes pipelining techniques and multiple functional units.
    Parallel processing using multi-processors will be covered in Unit
    8.  
      
     Reading this article should take approximately 15 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Charles Severance and Kevin Dowd, and the original can
    be found [here](http://cnx.org/content/m32775/latest/).

-   **Reading: Wikipedia: “Instruction-Level Parallelism”**
    Link: Wikipedia: [“Instruction-Level
    Parallelism”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-5.7-Instruction-levelparallelism-Wikipediathefreeencyclopedia-CCBYNCSA_files/CS301-5.7-Instruction-levelparallelism-Wikipediathefreeencyclopedia-CCBYNCSA.html) (HTML)  
      
     Instructions: Read the explanation of instruction level
    parallelism. Parallelism can occur at different levels of
    granularity, and when discussing parallelism, we need to be clear on
    exactly what is being done in parallel.  
      
     Reading this article should take approximately 15 minutes.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Instruction-level_parallelism).

**The Saylor Foundation’s “Unit 5 Assessment”** <span id="5.8"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 5 Assessment: Designing
    a Processor”**
    Link: The Saylor Foundation’s [“Unit 5 Assessment: Designing a
    Processor”](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-5.FINAL_.pdf)
    (PDF)  
        
     Instructions: Complete this assessment to test your knowledge of
    the concepts and learning outcomes in Unit 5. As you complete this
    assessment, take some time to think about architecture, computer
    architecture, von Neumann architecture, and a design that implements
    the architecture. Once you have completed the assessment, or if you
    need help, refer to the [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-5-AnswerKey-FINAL.pdf).  
      
     Completing this assessment should take approximately 3 hours.


