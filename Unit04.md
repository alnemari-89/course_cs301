---
layout: default
title: "CS301: Computer Architecture"
course_description: "An exploration of the basic hardware/software components, assembly language, and functional architecture design of computers."
next: ../Unit05
previous: ../Unit03
---
**Unit 4: Computer Arithmetic** <span id="4"></span> 
*In this unit, you will build upon your knowledge of computer
instructions and digital logic design to discuss the role of computer
arithmetic in hardware design. We will also discuss the designs of
adders, multipliers, and dividers. You will learn that there are two
types of arithmetic operations performed by computers: integer and
floating point. Finally, we will discuss the basics of floating point
representation for carrying out operations with real numbers.*

**Unit 4 Time Advisory**  
Completing this unit should take approximately 13 hours.  
  
 ☐    Subunit 4.1: 2 hours  
  
 ☐    Subunit 4.2: 2 hours  
  
 ☐    Subunit 4.3: 2 hours  
  
 ☐    Subunit 4.4: 2 hours  
  
 ☐    Subunit 4.5: 2 hours  
  
 ☐    Subunit 4.6: 1 hour  
  
 ☐    Unit 4 Assessment: 2 hours

**Unit4 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   discuss computer arithmetic hardware blocks and floating point
    representation;  
      
-   explain the representation of information, in particular integers
    and floating point numbers in a computer register or memory word;  
      
-   explain how arithmetic computations, addition, multiplication,
    subtraction, and division are performed on the data stored in a
    computer word;  
      
-   explain how to design simple hardware components, such as a half
    adder and full adder, perform this task, and in turn, use these
    components to perform subtraction and multiplication; and  
      
-   discuss the relationship of software and the hardware it controls.

**4.1 Number Representation** <span id="4.1"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 3: “Computer
    Arithmetic”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 3: Computer
    Arithmetic”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read sections 3.1 and 3.2 on pages 88–94 on
    representation of integers and real numbers. In subunit 2.2, you
    have previously read about number systems and the representation of
    numbers used for computing. This reading will give you a chance to
    review that material.   
      
     Computer architecture comprises components which perform the
    functions of storage of data, transfer of data from one component to
    another, computations, and interfacing to devices external to the
    computer. Data is stored in terms of units, called words. A word is
    made up of a number of bits, typically, depending on the computer,
    32 bits or 64 bits. Words keep getting longer, i.e., larger number
    of bits. Instructions are also stored in words. In previous
    subunits, you have seen examples of how instructions are stored in a
    word or words. In this subunit, you will see how numbers are stored
    in words.  
        
     Reading these sections should take approximately 1 hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html). 

-   **Reading: Wikipedia: “Floating Point”**
    Link: Wikipedia: [“Floating
    Point”](http://www.saylor.org/site/wp-content/uploads/2011/05/floating-point.pdf)(PDF)  
        
     Instructions: This reading supplements the prior reading on
    representation of real numbers. Read the sections titled “Overview,”
    “Range of Floating-Point Numbers,” “History,” “IEEE 754,” and
    “Representable Numbers” on pages 1–8.  
        
     Reading these sections should take approximately 1 hour.  
        
     Terms of Use: The article above is released under
    a [CreativeCommonsAttribution-Share-AlikeLicense3.0](http://creativecommons.org/licenses/by-sa/3.0/).
    You can find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Floating_point).

**4.2 Addition and Subtraction Hardware** <span id="4.2"></span> 
-   **Lecture: University of California, Santa Barbara: Professor
    Behrooz Parhami’s “Part II: Addition”**
    Link: University of California, Santa Barbara: Professor Behrooz
    Parhami’s [“Part II:
    Addition”](http://www.saylor.org/site/wp-content/uploads/2011/09/CS301-Sub4.1-PartII-Addition.pdf) (PDF)  
      
     Instructions: Study slides 1–29 from Chapter 5 to learn how
    addition is implemented and carried out at the gate level. In the
    state of the practice, i.e., in the current profession, computers
    are architected using larger components. For example, to perform
    addition and subtraction, computer architects utilize ALU’s,
    arithmetic logic units. You can design a computer without knowing
    the details of an ALU or of an adder, similar to using a calculator
    to find the square root of a number without knowing how to manually
    compute the square root (or in computer science terminology, without
    knowing the algorithm that the calculator performs to find the
    square root). However, we want you to have the strongest foundation
    in your study of computer architecture. Hence, study the assigned
    slides for Chapter 5. If you feel very ambitious, optionally you can
    study Chapters 6–8, which expand on basic addition.  
      
     Knowing the underlying algorithm for larger components, you will be
    able to better use them in constructing larger components, for
    example, using half adders to construct a full adder. A half adder
    takes 2 bits as input and outputs a sum and a carry bit; a full
    adder takes 2 operand bits and a carry bit as input, and outputs a
    sum bit and a carry bit. Note that to add two floating pint numbers,
    one or both need to be put in a form such that they have the same
    exponent. Then, the mantissas are added. Lastly, the result is
    normalized. We will cover floating point addition in subunit 4.4.
    Subtraction is not discussed explicitly, because it is done via
    addition by reversing the sign of the number to be subtracted
    (subtrahend) and adding the result to the number subtracted from
    (minuend). You have to be careful when subtracting floating point
    numbers, because of the possible large roundoff error in the
    result.  
        
     Studying this chapter should take approximately 2 hours. You should
    dedicate approximately 3 additional hours if you choose to review
    the optional material.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Professor Behrooz Parhami and can be viewed in
    its original
    form [here](http://www.ece.ucsb.edu/~parhami/text_comp_arit.htm).
    Please note that this material is under copyright and cannot be
    reproduced in any capacity without explicit permission from the
    copyright holder.

**4.3 Multiplication** <span id="4.3"></span> 
-   **Web Media: University of California, Santa Barbara: Professor
    Behrooz Parhami’s “Part III: Multiplication”**
    Link: University of California, Santa Barbara: Professor Behrooz
    Parhami’s [“Part III:
    Multiplication”](http://www.saylor.org/site/wp-content/uploads/2011/09/CS301-Sub-Part-III-Multiplication.pdf) (PDF)  
        
     Instructions: Study slides 1–26 from Chapter 9. In particular,
    focus on section 9.1 to learn how multiplication is performed using
    basic steps that are carried out by elemental logic components, such
    as an adder and shifter. Two numbers are loaded into registers (fast
    word storage) and multiplication is carried out by repeated addition
    and shifting (moving the bits in a register to the right or left).
    The presentation first shows how multiplication is done for unsigned
    integers and then how signed numbers are handled.   
      
     When you read the slides, follow along by using a pad of paper and
    multiply two small binary numbers. Note k is the position of the
    binary digit; from right to left, k takes on 0, 1, 2, etc. j is the
    partial product; j goes from 1, 2, 3, etc. However, for consistency
    the 0th partial product is defined to be 0. Chapters 10–12 are
    optional; these chapters discuss ways of speeding up
    multiplication.  
      
     Note that to multiply two floating point numbers, add the
    exponents, multiply the mantissas, normalize the mantissa of the
    product, and adjust the exponent accordingly. Floating point
    multiplication will be covered in a following subunit 4.4.  
        
     Reading this chapter should take approximately 2 hours. You should
    dedicate approximately 3 additional hours, if you choose to review
    the optional material.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Professor Behrooz Parhami and can be viewed in
    its original
    form [here](http://www.ece.ucsb.edu/~parhami/text_comp_arit.htm).
    Please note that this material is under copyright and cannot be
    reproduced in any capacity without explicit permission from the
    copyright holder.

**4.4 Floating Point Arithmetic** <span id="4.4"></span> 
-   **Reading: Wikipedia: “Floating Point”**
    Link: Wikipedia: [“Floating
    Point”](http://www.saylor.org/site/wp-content/uploads/2011/05/floating-point.pdf)(PDF)  
      
     Instructions: Read the sections titled “Floating Point Arithmetic
    Operations,” “Dealing with Exceptional Cases,” and “Accuracy
    Problems” on pages 9–15. This is a continuation of the reading from
    subunit 4.1. The prior reading dealt with representation of real
    numbers. This reading extends the discussion to operations on
    floating point numbers.  
        
     Reading these sections should take approximately 1 hour.  
        
     Terms of Use: The article above is released under
    a [CreativeCommonsAttribution-Share-AlikeLicense3.0](http://creativecommons.org/licenses/by-sa/3.0/).
    You can find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Floating_point).

-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 3: Computer
    Arithmetic”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 3: Computer
    Arithmetic”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read section 3.3 on pages 94–100 and section 3.4 on
    pages 100–102. Section 3.3 provides an additional explanation of
    error analysis when numbers are represented using a fixed number of
    digits. This issue mostly arises when using floating point
    numbers. Real numbers are represented using a fixed number of
    bits. The number of bits is the precision of the representation. The
    accuracy of the representation is described in terms of the
    difference between the actual number and its representation using a
    fixed number of bits. This difference is the error of the
    representation. The accuracy becomes more significant, because
    computations can cause the error to get so large that the result is
    meaningless and potentially even high risk depending on the
    application. Section 3.4 explains how programming languages approach
    number representation.  
        
     Reading these sections should take approximately 1 hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**4.5 Division** <span id="4.5"></span> 
-   **Reading: University of California, Santa Barbara: Professor
    Behrooz Parhami’s “Part IV: Division”**
    Link: University of California, Santa Barbara: Professor Behrooz
    Parhami’s [“Part IV:
    Division”](http://www.saylor.org/site/wp-content/uploads/2011/09/CS301-Part-IV-Division.pdf) (PDF)   
      
     Instructions: Study slides 1–34 from Chapter 13. In particular,
    focus on section 13.1, which explain the basics of division using
    subtraction and shifting. Chapters 14–16 are optional; these
    chapters cover ways of speeding up division.  
        
     Studying this chapter should take approximately 2 hours. You should
    dedicate approximately 3 additional hours if you choose to review
    the optional material.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Behrooz Parhami and can be viewed in its original
    form [here](http://www.ece.ucsb.edu/~parhami/text_comp_arit.htm).
    Please note that this material is under copyright and cannot be
    reproduced in any capacity without explicit permission from the
    copyright holder.

**4.6 Case Study: Floating Point Arithmetic in an x86 Processor** <span
id="4.6"></span> 
-   **Reading: Wikipedia: “Extended Precision”**
    Link: Wikipedia: [“Extended
    Precision”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-4.6-Extendedprecision-Wikipediathefreeencyclopedia-CCBYNCSA_files/CS301-4.6-Extendedprecision-Wikipediathefreeencyclopedia-CCBYNCSA.html)
    (HTML)  
        
     Instructions: Read this article to learn about minimizing roundoff
    and overflow in floating point arithmetic using extended
    precision.  
        
     Reading this article and taking notes should take approximately 1
    hour.  
        
     Terms of Use: The article above is released under
    a [CreativeCommonsAttribution-Share-AlikeLicense3.0](http://creativecommons.org/licenses/by-sa/3.0/).
    You can find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Extended_precision).

**The Saylor Foundation’s “Unit 4 Assessment"** <span id="4.7"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 4 Assessment: Computer
    Arithmetic”**
    Link: The Saylor Foundation’s [“Unit 4 Assessment: Computer
    Arithmetic”](http://www.saylor.org/site/wp-content/uploads/2012/07/CS301-Computer-Architecture-Assessment-4.FINAL_.pdf)
    (PDF)  
      
     Instructions: Complete this assessment to test your knowledge of
    the concepts and learning outcomes in Unit 4. Once you have
    completed the assessment, or if you need help, refer to the [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/07/CS301-Computer-Architecture-Assessment-4-Answer-Key.FINAL_.pdf).  
      
     Completing this assessment should take approximately 2 hours.


