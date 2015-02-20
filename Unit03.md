**Unit 3: Fundamentals of Digital Logic Design** <span id="3"></span> 
*We will begin this unit with an overview of digital components,
identifying the building blocks of digital logic. We will build on that
foundation by writing truth tables and learning about more complicated
sequential digital systems with memory. This unit serves as background
information for the processor design techniques we learn in later
units. *

**Unit 3 Time Advisory**  
Completing this unit should take approximately 16.5 hours.  
  
 ☐    Subunit 3.1: 1.25 hours  
  
 ☐    Subunit 3.2: 3 hours  
  
 ☐    Subunit 3.3: 3 hours  
  
 ☐    Subunit 3.4: 6 hours  
  
 ☐    Subunit 3.5: 0.25 hours  
  
 ☐    Unit 3 Assessment: 3 hours

**Unit3 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   describe the process of carrying out sequential logic design; and  
      
-   describe the evolution of physical components used to implement
    Boolean logic in the design of digital processors and computers.

**3.1 Beginning Design: Logic Gates, Truth Table, and Logic Equations**
<span id="3.1"></span> 
-   **Reading: Massachusetts Institute of Technology: Jerome H. Saltzer
    and M. Frans Kaashoek’s *Principles of Computer System Design: An
    Introduction*: “Design Principles”**
    Link: Massachusetts Institute of Technology: Jerome H. Saltzer and
    M. Frans Kaashoek’s *Principles of Computer System Design: An
    Introduction*: [“Design
    Principles”](http://ocw.mit.edu/resources/res-6-004-principles-of-computer-system-design-an-introduction-spring-2009/online-textbook/)
    (PDF)  
        
     Instructions: Click on the PDF link for “Design Principles,” and
    study these principles. This reading provides a list of important
    design principles, applicable to any type of design and, in
    particular to computer system design, software or hardware. Consider
    these principles as well as other design considerations as a guide
    to computer system design.  
        
     Studying these principles should take approximately 15 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-sa/3.0/). It is
    attributed to Jerome H. Saltzer and M. Frans Kaashoek, and the
    original version can be found
    [here](http://ocw.mit.edu/resources/res-6-004-principles-of-computer-system-design-an-introduction-spring-2009/online-textbook/). 

-   **Reading: Wikipedia: “Logic Gates”**
    Link: Wikipedia: [“Logic
    Gates”](http://www.saylor.org/site/wp-content/uploads/2011/05/logic-gate.pdf) (PDF)  
      
     Instructions: Read this article, paying particular attention to the
    sections titled “Background,” “Logic Gates,” “Symbols,” “De Morgan
    Equivalent Symbols,” and “Three-State Logic Gates.” Logic devices
    are physical implementations of Boolean logic and are built from
    components, which have gotten larger and more complex over time, for
    example: relays and transistors, gates, registers, multiplexors,
    adders, multipliers, ALUs (arithmetic logic units), data buses,
    memories, interfaces, and processors. These devices respond to
    control and data signals specified in machine instructions to
    perform the functions for which they were designed.  
      
     Reading this article should take approximately 1 hour.  
      
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/). You can find
    the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Logic_gate).

**3.2 Combinational Logic** <span id="3.2"></span> 
-   **Reading: iBiblio: Tony R. Kuphalt’s *Lessons in Electric Circuits,
    Volume IV*: “Chapter 9: Combinational Logic Functions” and “Chapter
    6: Ladder Logic”**
    Link: iBiblio: Tony R. Kuphalt’s *Lessons in Electric Circuits,
    Volume IV*: [“Chapter 9: Combinational Logic
    Functions”](http://www.saylor.org/site/wp-content/uploads/2011/06/CS301-3.2.pdf)
    (PDF) and [“Chapter 6:
    Ladder Logic”](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_6.html)
    (HTML)  
      
     Instructions: First, read Chapter 9, which describes the design of
    several components using logic gates, including adders, encoders and
    decoders, multiplexers, and demultiplexers. This chapter also
    mentions ladder logic. If you are not familiar with ladder logic,
    use Chapter 6 as a reference. Note that Chapter 6 is an optional
    resource.  
      
     Reading this chapter should take approximately 3 hours. You should
    dedicate approximately 2 additional hours if you read and refer to
    the optional chapter.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Tony R. Kuphaldt, and can be viewed in its
    original from
    [here](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_9.html).
    Please note that this material is under copyright and cannot be
    reproduced in any capacity without explicit permission from the
    copyright holder.

**3.3 Flip-Flops, Latches, and Registers** <span id="3.3"></span> 
-   **Reading: iBiblio: Tony R. Kuphalt’s *Lessons in Electric Circuits,
    Volume IV*: “Chapter 10: Multivibrators”**
    Link: iBiblio: Tony R. Kuphalt’s *Lessons in Electric Circuits,
    Volume IV*: [“Chapter 10:
    Multivibrators”](http://www.saylor.org/site/wp-content/uploads/2011/06/CS301-3.3.pdf) (PDF)  
      
     Instructions: Read Chapter 10, which discusses how logic gates are
    connected to store bits, i.e., 0’s and 1’s. Combinational circuits,
    described in the previous section, do not have memory. Using logic
    gates, latches and flip flops are designed for storing bits. Groups
    of flip flops are used to build registers which hold strings of
    bits. For each storage device in Chapter 10, focus on the overview
    at the beginning of the section and the review of the device’s
    characteristics at the end of its section. While you do not
    absolutely need to know the details of how latches and flip flops
    work, you might find the material of interest. We strongly recommend
    that you read the details of the design of each storage device,
    because it will give you a stronger background.  
      
     Reading this chapter should take approximately 3 hours.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Tony R. Kuphalt and can be viewed in its original
    from
    [here](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_10.html). Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**3.4 Sequential Logic Design** <span id="3.4"></span> 
-   **Reading: iBiblio: Tony R. Kuphalt’s *Lessons in Electric Circuits,
    Volume IV*: “Chapter 11: Finite State Machines” and “Chapter 8:
    Karnaugh Mapping”**
    Link: iBiblio: Tony R. Kuphalt’s *Lessons in Electric Circuits,
    Volume IV*: [“Chapter 11: Sequential
    Circuits”](http://www.saylor.org/site/wp-content/uploads/2011/06/CS301-3.4.pdf) (PDF)
    and [“Chapter 8: Karnaugh
    Mapping”](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_8.html) (HTML)  
      
     Instructions: First, read Chapter 11 on sequential circuits.
    Combinatorial circuits, discussed in a previous unit, have outputs
    that depend on the inputs. Sequential circuits and finite state
    machines have outputs that depend on the inputs AND the current
    state, values stored in memory. Then, read Chapter 8 on Karnaugh
    mapping, a tabular way for simplifying Boolean logic. There are
    several ways for representing Boolean logic: algebraic expressions
    which use symbols and Boolean operations; Venn diagrams which use
    distinct and overlapping circles; and tables relating inputs to
    outputs (for combinational logic) or tables relating inputs and
    current state to outputs and next state (for sequential logic). When
    designing sequential logic, some of the components are memory
    devices. Cost and processing time are considerations in using memory
    devices, which can be expensive. To reduce the cost or processing
    time the logic can be simplified. This simplification can be done
    using algebraic rules to manipulate the symbols and operations,
    analysis of the areas inside the circles for Venn diagrams, or
    Karnaugh maps for input/output tables. Some of you may be familiar
    with Karnaugh mapping from previous courses or work experience.   
      
     Reading these chapters should take approximately 6 hours.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Tony R. Kuphalt and can be viewed in its original
    from
    [here](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_11.html#xtocid90934)
    and
    [here](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_8.html). Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**3.5 Case Study: Design of a Finite State Machine (FSM) to Control a
Vending Machine** <span id="3.5"></span> 
-   **Reading: The Saylor Foundation’s “Finite State Automata”**
    Link: The Saylor Foundation’s [“Finite State
    Automata”](http://www.saylor.org/site/wp-content/uploads/2011/06/CS-202-Subunit-9.2-Finite-State-Automata_FINAL.pdf) (PDF)  
      
     Instructions: Read this article for an example of a finite state
    machine design of a simple vending machine.  
        
     A sequential circuit is also called a sequential machine or a
    finite state machine (FSM) or a finite state automaton. This case
    study gives an example that illustrates the concepts of this unit
    for the design of a sequential circuit. A binary table represents
    the input/output behavior of the circuit. We use a sequential
    circuit, because the output also depends on the state. Recall from
    your readings, that state requires memory, i.e., flip flops. Thus, a
    binary table with entries that give the output and next state for
    given inputs and current state represents the design of the
    machine. A finite state machine diagram can also represent the
    design: circles represent states; arrows represent transitions next
    to states; and inputs and outputs label the arrows (sometimes
    written as input/ output). Finally, Boolean equations can also
    represent the design. Lastly, Karnaugh maps or Boolean logic rules
    can be used to simplify, i.e., minimize, the equations and, thus,
    the design.  
        
     Reading this article should take approximately 15 minutes.

**The Saylor Foundation’s “Unit 3 Assessment”** <span id="3.6"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 3 Assessment:
    Fundamentals of Digital Logic Design”**
    Link: The Saylor Foundation’s [“Unit 3 Assessment: Fundamentals of
    Digital Logic
    Design”](http://www.saylor.org/site/wp-content/uploads/2012/07/CS301-Computer-Architecture-Assessment-3.FINAL_.pdf)
    (PDF)  
                  
     Instructions: Complete this assessment to test your knowledge of
    the concepts and learning outcomes for Unit 3. As you complete this
    assessment, you will look at combinational circuit design and
    sequential circuit design. Once you have completed the assessment,
    or if you need help, refer to the [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/07/CS301-Computer-Architecture-Assessment-3-Answer-Key.FINAL_.pdf).  
      
     Completing this assessment should take approximately 3 hours.


