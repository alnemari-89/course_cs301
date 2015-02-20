**Unit 2: Instructions: Hardware Language** <span id="2"></span> 
**In order to understand computer architecture, you need to understand
the components that comprise a computer and their interconnections. Sets
of instructions, called* *programs,* *describe the computations that
computers carry out. The instructions are strings of binary digits. When
symbols are used for the binary strings, the instructions are called*
*assembly languageinstructions. Components interpret the instructions
and send signals to other components that cause the instruction to be
carried out.*  
    
 *In this unit, you will build on your knowledge of programming from*
[CS102](http://www.saylor.org/courses/cs102/) *to learn how to program
with an assembly language. You will use the instructions of a real
processor, MIPS, to understand the basics of hardware language. We will
also discuss the different classes of instructions typically found in
computers and compare the MIPS instructions to those found in other
popular processors made by Intel and ARM.**

**Unit 2 Time Advisory**  
Completing this unit should take approximately 14 hours.  
  
 ☐    Subunit 2.1: 1 hour  
  
 ☐    Subunit 2.2: 5 hours  
  
 ☐    Subunit 2.3: 1.5 hours  
  
 ☐    Subunit 2.4: 0.5 hours  
  
 ☐    Subunit 2.5: 0.25 hours  
  
 ☐    Subunit 2.6: 0.25 hours  
  
 ☐    Subunit 2.7: 1.5 hours  
  
 ☐    Subunit 2.8: 2 hours  
  
 ☐    Unit 2 Assessment: 2 hours

**Unit2 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   explain how programs written in high-level programming language,
    such as C or Java, can be translated into the language of the
    hardware; and  
      
-   describe the interface between hardware and software, and explain
    how software instructs hardware to accomplish desired functions.

**2.1 Computer Hardware Operations** <span id="2.1"></span> 
-   **Reading: University of Maryland, Baltimore Country: Dr. Jon
    Squire’s “Computer Operations”**
    Link: University of Maryland, Baltimore Country: Dr. Jon Squire’s
    [“Computer
    Operations”](http://www.saylor.org/site/wp-content/uploads/2011/06/CS301-2.1.pdf) (PDF)  
      
     Instructions: Study these lecture notes to learn about the basic
    operations, or machine instructions, of a computer processor.  
      
     Studying these lecture notes should take approximately 1 hour.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Dr. Jon Squire and can be viewed in its original
    from [here](http://www.cs.umbc.edu/~squire/cs411_l4.html). Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**2.2 Number Representation in Computers** <span id="2.2"></span> 
-   **Reading: University of California, Santa Barbara: Professor
    Behrooz Parhami’s “Part I: Number Representation”**
    Link: University of California, Santa Barbara: Professor Behrooz
    Parhami’s [“Part I: Number
    Representation”](http://www.saylor.org/site/wp-content/uploads/2011/09/CS301-sub2.2-Numer-Representatio.pdf) (PDF)  
      
     Instructions: Read Chapter 1 and Chapter 2 of part I up to slide
    37. These lecture notes explain how numbers are represented, i.e.,
    encoded by using a string of bits – or binary digits. These lecture
    notes also describe how the sign of a number is represented and how
    2’s complement representation. Finally, skim slides 38–88 to get a
    basic understanding of what they cover: redundant number systems and
    residue number systems. This material may or may not be difficult,
    depending on your mathematical background; make sure to take your
    time as you study this material.  
      
     Studying these lecture notes should take approximately 3 hours.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Professor Behrooz Parhami and can be viewed in
    its original form
    [here](http://www.ece.ucsb.edu/~parhami/text_comp_arit.htm). Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder.  

-   **Reading: iBiblio: Tony R. Kuphalt’s Lessons in Electric Circuits,
    Volume IV: “Chapter 1: Numeration Systems”**
    Link: iBiblio: Tony R. Kuphalt’s Lessons in Electric Circuits,
    Volume IV: [“Chapter 1: Numeration
    Systems”](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_1.html)
    (PDF)  
        
     Instructions: Read Chapter 1 on numeration systems. This is an
    alternative reading for number representation used for digital
    hardware devices.   
      
     Reading this chapter should take approximately 2 hours.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Tony R. Kuphaldt and can be viewed in its
    original from
    [here](http://www.ibiblio.org/kuphaldt/electricCircuits/Digital/DIGI_1.html).
    Please note that this material is under copyright and cannot be
    reproduced in any capacity without explicit permission from the
    copyright holder.

**2.3 Instruction Representation** <span id="2.3"></span> 
-   **Reading: Wikibooks: “MIPS Assembly/Instruction Formats”**
    Link: Wikibooks: [“MIPS Assembly/Instruction
    Formats”](http://www.saylor.org/site/wp-content/uploads/2011/05/MIPS_AssemblyInstruction_Formats.pdf) (PDF)  
      
     Instructions: Read this article for an introduction to the three
    different instruction formats for the MIPS processor: the R-Format,
    the I-Format, and the J-Format instructions. MIPS is an acronym that
    stands for Microprocessor Instructions without Interlocked Pipeline
    Stages. MIPS is a RISC (Reduced Instruction Set Computer) introduced
    by MIPS technologies. Also, ISA, if you encounter it, stands for
    Instruction Set Architecture.  
      
     Reading this article should take approximately 1 hour and 30
    minutes.  
      
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/). You can find
    the original Wikibooks version of this
    article [here](http://en.wikibooks.org/wiki/MIPS_Assembly/Instruction_Formats).

**2.4 Logical and Arithmetic Instructions** <span id="2.4"></span> 
-   **Reading: Wikibooks: “MIPS Assembly/Arithmetic Instructions”**
    Link: Wikibooks: [“MIPS Assembly/Arithmetic
    Instructions”](http://www.saylor.org/site/wp-content/uploads/2011/05/MIPS_AssemblyArithmetic_Instructions.pdf) (PDF)  
      
     Instructions: Read this article to learn about arithmetic and
    logical instructions for the MIPS processor.   
      
     Reading this article should take approximately 30 minutes.  
      
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/). You can find
    the original Wikibooks version of this
    article [here](http://en.wikibooks.org/wiki/MIPS_Assembly/Arithmetic_Instructions).

**2.5 Control Instructions** <span id="2.5"></span> 
-   **Reading: Wikibooks: “MIPS Assembly/Control Flow Instructions”**
    Link: Wikibooks: [“MIPS Assembly/Control Flow
    Instructions”](http://www.saylor.org/site/wp-content/uploads/2011/05/MIPS_AssemblyControlFlowInstructions.pdf)
    (PDF)  
      
     Instructions: Read this article to learn about the control flow
    instructions for the MIPS processor, including the basic ones: jump
    and branch instructions.  
      
     Reading this article should take approximately 15 minutes.  
      
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/). You can find
    the original Wikibooks version of this article
    [here](http://en.wikibooks.org/wiki/MIPS_Assembly/Control_Flow_Instructions).

**2.6 Instructions for Memory Operations** <span id="2.6"></span> 
-   **Reading: Wikibooks: “MIPS Assembly/Memory Instructions”**
    Link: Wikibooks: [“MIPS Assembly/Memory
    Instructions”](http://www.saylor.org/site/wp-content/uploads/2011/05/MIPS-Assembly-Memory-Instructions.pdf)
    (PDF)  
      
     Instructions: Read this article to learn about memory instructions
    for the MIPS processor.   
      
     Reading this article should take approximately 15 minutes.  
      
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/). You can find
    the original Wikibooks version of this article
    [here](http://en.wikibooks.org/wiki/MIPS_Assembly/Memory_Instructions).

**2.7 Different Modes for Addressing Memory** <span id="2.7"></span> 
-   **Reading: Wikipedia: “Addressing Mode”**
    Link: Wikipedia: [“Addressing
    Mode”](http://www.saylor.org/site/wp-content/uploads/2011/05/Addressing-mode.pdf)
    (PDF)  
      
     Instructions: Read this article to study the various formats for
    addressing memory.  
      
     Reading this article should take approximately 1 hour.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Addressing_mode).

-   **Reading: Wikibooks: MIPS Assembly: “Instruction Format”**
    Link: Wikibooks: *MIPS Assembly*: [“Instruction
    Format”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-2.7-MIPSAssemblyInstructionFormats-Wikibooksopenbooksforanopenworld-CCBYNCSA_files/CS301-2.7-MIPSAssemblyInstructionFormats-Wikibooksopenbooksforanopenworld-CCBYNCSA.html)
    (HTML)  
        
     Instructions: Read this section titled “Instruction Format.” MIPS
    assembly is an assembly language, which is a mnemonic or meaningful
    code for the machine language format in computer programming. Read
    this section to get a sense of how the addresses to memory are coded
    in a MIPS microprocessor.  
        
     Reading this section should take approximately 30 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikibooks version of this
    article [here](http://en.wikibooks.org/wiki/MIPS_Assembly/Instruction_Formats).

**2.8 Case Study: Intel and ARM Instructions** <span id="2.8"></span> 
-   **Reading: Wikibooks: X86 Assembly: “X86 Instructions” and
    Wikibooks: “ARM Architecture”**
    Link: Wikibooks: *X86 Assembly*: [“X86
    Instructions”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-2.8-X86AssemblyX86Instructions-Wikibooksopenbooksforanopenworld-CCBYNCSA_files/CS301-2.8-X86AssemblyX86Instructions-Wikibooksopenbooksforanopenworld-CCBYNCSA.html)
    (HTML) and Wikibooks: [“ARM
    Architecture”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS3-1-2.8-ARMarchitecture-Wikipediathefreeencyclopedia-CCBYNCSA_files/CS3-1-2.8-ARMarchitecture-Wikipediathefreeencyclopedia-CCBYNCSA.html)
    (HTML)  
        
     Instructions: Read the article titled “X86 Instructions.” For “ARM
    Architecture,” read the “Instruction Set” section, stopping at
    “Debugging.” These articles provide two examples of instructions set
    architectures (ISAs). Look over how the different microprocessors
    address memory. Take note of similarities and differences of format,
    instructions and type of instructions, and addressing modes between
    these two as well as between these and the MIPS instructions of the
    previous sections.  
      
     Reading these articles should take approximately 2 hours.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikibooks version of this articlehere.

**The Saylor Foundation’s “Unit 2 Assessment”** <span id="2.9"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 2 Assessment: Hardware
    Language”'**
    Link: The Saylor Foundation’s [“Unit 2 Assessment: Hardware
    Language”](http://www.saylor.org/site/wp-content/uploads/2012/09/CS301-Computer-Architecture-Assessment-2.FINAL_.pdf)
    (PDF)  
      
     Instructions: Complete this assessment to test your knowledge on
    the concepts and learning outcomes for Unit 2. As you complete this
    assessment, you will take a closer look at the software/hardware
    interface and evaluate the fundamental idea of a general purpose
    machine. Once you have completed the assessment, or if you need
    help, refer to the [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/09/CS301-Computer-Architecture-Assessment-2-Answer-Key.FINAL_.pdf).
       
      
     Completing this assessment should take approximately 2 hours.


