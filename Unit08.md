<<<<<<< HEAD
---
layout: default
title: "CS301: Computer Architecture"
course_description: "An exploration of the basic hardware/software components, assembly language, and functional architecture design of computers."
next: ../Unit09
previous: ../Unit07
---
=======
>>>>>>> master
**Unit 8: Parallel Processing** <span id="8"></span> 
*This unit will address several advanced topics in computer
architecture, focusing on the reasons for and the consequences of the
recent switch from sequential processing to parallel processing by
hardware producers. You will learn that parallel programming is not
easy and that parallel processing imposes certain limitations in
performance gains, as seen in the well-known Amdahl’s law. You will also
look into the concepts of shared memory multi-processing and cluster
processing as two common means of improving performance with
parallelism. The unit will conclude with a look at some of the
programming techniques used in the context of parallel machines.*

**Unit 8 Time Advisory**  
Completing this unit should take approximately 18.25 hours.  
  
 ☐    Subunit 8.1: 1.25 hours  
  
 ☐    Subunit 8.2: 2 hours  
  
 ☐    Subunit 8.3: 2 hours  
  
 ☐    Subunit 8.4: 11 hours   
  
 ☐    Unit 8 Assessment: 2 hours

**Unit8 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   identify reasons for and consequences of the recent switch from
    sequential processing to parallel processing amongst hardware
    manufacturers;  
      
-   explain the basics of parallel programming; and  
      
-   describe the approaches to parallelism used to improve performance
    and overcome the limits of current physical devices and their
    fabrication.

**8.1 The Reason for the Switch to Parallel Processing** <span
id="8.1"></span> 
*The video lecture assigned below subunit 1.5 covers this topic. Review
this video lecture and your notes for an understanding of the reasons
behind the switch to parallel computing. Now that you have gone through
most of the course, you will have a better appreciation of the change
that is taking place today. This great motivational lecture provides
insight into parallel architecture trends and research.* *Take
approximately 1 hour to review this lecture and your notes.*

-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 1: Sequential
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 1: Sequential
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read section 1.3 of Chapter 1 on pages 23 and 24 to
    learn about multi-core chips. These two pages give a summary of
    processor and chip trends to overcome the challenge of increasing
    performance and addressing the heat problem of a single core.  
        
     Reading this section should take approximately 15 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**8.2 Limitations in Parallel Processing: Amdahl’s Law** <span
id="8.2"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 2: Parallel
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing: *[“Chapter 2: Parallel
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read sections 2.1 and 2.2 of Chapter 2 on pages 41–45
    to learn about parallel computer architectures. There are different
    types of parallelism: there is instruction-level parallelism, where
    a stream of instructions is simultaneously in partial stages of
    execution by a single processor; there are multiple streams of
    instructions, which are simultaneously executed by multiple
    processors. The former was addressed in Unit 5. The latter is
    addressed in this reading. A quote from the beginning of the chapter
    states the key ideas: “In this chapter, we will analyze this more
    explicit type of parallelism, the hardware that supports it, the
    programming that enables it, and the concepts that analyze it.” This
    reading begins with a simple scientific computation example,
    followed by a description of SISD, SIMD, MISD, and MIMD
    architectures.  
      
     Reading these sections should take approximately 30 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

-   **Reading: Ariel Ortiz Ramírez’s “Parallelism and Performance”**
    Link: Ariel Ortiz Ramírez’s [“Parallelism and
    Performance”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-8.2-ParallelismandPerformance-CCBYNCSA_files/CS301-8.2-ParallelismandPerformance-CCBYNCSA.html) (HTML)  
      
     Instructions: Study the section titled “Amdahl’s Law.” *Amdahl’s
    law* explains the limitations to performance gains achievable
    through parallelism. Over the last several decades or so, increases
    in computer performance have largely come from improvements to
    current hardware technologies and less from software
    technologies. Now, however, the limits to these improvements may be
    near. For significant continued performance improvement, either new
    physical technology needs to be discovered and/or transitioned to
    practice, or software techniques will have to be developed to get
    significant gains in computing performance.  
      
     In the equation for Amdahl’s law, P is the fraction of code that
    can be parallelized, i.e., that must be executed serially; S is the
    fraction of code that cannot be parallelized; and n is the number of
    processors. Note P + S is 1. If there are n processors, then P + S
    can be executed in the same time that P/n + S can be executed. Thus,
    the ratio of the time using 1 processor to the time of using n
    processors is 1/(P/n + S). This is the speedup in going from 1
    processor to n processors.  
      
     Note that the speedup is limited, even for large n. If n is 1, the
    speedup is 1. If n is very large, then the speedup is 1/S. If P is
    very small, then P/n is even smaller, and P/n + S is approximately
    S, i.e., the speedup is 1/S, but S is approximately S + P, which is
    1. Therefore, the speed of execution of this code using 1 processor
    is about the same as using n processors.  
      
     Another way of writing Amdahl’s law is 1/(P/n + [1 – P]). Thus, if
    P is close to 1, the speedup is 1/(P/n) or n/P, which is
    approximately n.  
      
     Apply Amdahl’s law to better understand how it works by
    substituting a variety of numeric values into this equation and
    sketching the graph of the equation.  
      
     Studying this section and applying Amdahl’s law should take
    approximately 1 hour.  
      
     Terms of Use:This resource is licensed under a [Creative Commons
    Attribution-NonCommercial 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc/3.0/). It is
    attributed to Ariel Ortiz Ramírez, and the original version can be
    found
    [here](http://webcem01.cem.itesm.mx:8005/apps/s201311/tc5004/notes_parallelism/).
     

-   **Reading: Lawrence Livermore National Laboratory: Blaise Barney’s
    *Introduction to Parallel Computing*: “Chapter 6, Section 10: Limits
    and Costs of Parallel Programming”**
    Link: Lawrence Livermore National Laboratory: Blaise Barney’s
    *Introduction to Parallel Computing*: [“Chapter 6, Section 10:
    Limits and Costs of Parallel
    Programming”](https://computing.llnl.gov/tutorials/parallel_comp/#DesignCosts)
    (HTML)  
      
     Instructions: In section 10 of Chapter 6, study the section titled
    “Amdahl’s Law” up to the section titled “Complexity.” This reading
    will complement your study of Amdahl’s law from Ramírez’s article.  
        
     Studying this section should take approximately 30 minutes.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**8.3 Shared Memory and Distributed Memory Multiprocessing** <span
id="8.3"></span> 
-   **Reading: The Saylor Foundation’s “Multiprocessing”**
    Link: The Saylor Foundation’s
    [“Multiprocessing”](http://www.saylor.org/site/wp-content/uploads/2011/09/Multiprocessing.pdf) (PDF)  
      
     Instructions: Study these lecture slides. This reading focuses on
    the problem of parallel software. It discusses scaling, uses a
    single example to explain shared memory and message passing, and
    identifies problems related to cache and memory consistency.  
        
     Studying these lecture slides should take approximately 1 hour.

-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 2: Parallel
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing:* “[Chapter 2: Parallel
    Computer
    Architecture](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf)"
    (PDF)  
        
     Instructions: Read section 2.3 of Chapter 2 on pages 46 and 47 to
    learn about different types of memory access. Then, read section 2.4
    of Chapter 2 on pages 47–51 to learn about granularity of
    parallelism. A processor’s connections to memory affect its
    performance. Parallel machines can be connected to memory in
    different ways, so there are different ways to handle simultaneous
    access by multiple processors to the same memory location.
    Parallelism can be on various levels: control signal level (or
    micro-program instruction level), data level, computation level, or
    task level. This reading is a prelude to the next key topic of
    parallel programming in subunit 8.4.  
        
     Reading this section should take approximately 1 hour.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be
    found [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**8.4 Multicore Processors and Programming with OpenMP and MPI** <span
id="8.4"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 2: Parallel
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 2: Parallel
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read section 2.5 of Chapter 2 on pages 52–68. The
    reading covers two extreme approaches to parallel
    programming. First, parallelism is handled by the lower software and
    hardware layers. OpenMP is applicable in this first case. Secondly,
    parallelism is handled by the programmer. MPI is applicable in the
    second case.  
      
     This reading is a prelude to the topic of parallel programming,
    addressed in the following video lecture for this subunit.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

-   **Reading: Norm Matloff’s *Programming on Parallel Machines***
    Link: Norm Matloff’s *[Programming on Parallel
    Machines](http://heather.cs.ucdavis.edu/~matloff/158/PLN/ParProcBook.pdf)*
    (PDF)  
        
     Instructions: Read Chapter 1 on pages 1–20. If you go to the table
    of contents, selecting the section will jump you to the desired page
    to avoid scrolling through the text. Chapter 1 uses a matrix times
    (multiplication) vector example in section 1.3.1. This chapter goes
    on to describe parallel approaches for computing a solution: section
    1.3.2 describes a shared-memory and threads approach; section 1.3.3
    describes a message passing approach; section 1.3.4 describes the
    MPI and R language approach. Study these sections to get an overview
    of the idea of software approaches to parallelism.  
        
     Read Chapter 2 on pages 21 - 30. This chapter presents issues that
    slow the performance of parallel programs.  
      
     Read Chapter 3 on pages 31 - 66 to learn about shared memory
    parallelism. Parallel programming and parallel software are
    extensive topics and our intent is to give you an overview of them;
    more in depth study is provided by the following chapters.  
      
     Read Chapter 4 on pages 67 - 100. This chapter discusses MP
    directives and presents a variety of examples.  
      
     Read Chapter 5 on pages 101 - 136. This chapter presents GPUs
    (Graphic Processing Units) and the CUDA language. This chapter also
    discusses parallel programming issues in the context of GPUs and
    CUDA and illustrates them with various examples.  
      
     Read Chapter 7 on pages 161 - 166. This chapter illustrates the
    message passing approach using various examples.  
      
     Read Chapter 8 on pages 167 - 169 for a description of MPI (Message
    Passage Interface), which applies to networks of workstations
    (NOWs). The rest of the chapter illustrates this approach with
    various examples.   
      
     Read Chapter 9 on pages 193 - 206 for an overview of cloud
    computing and the hadoop platform, which are interesting topics for
    today not just for parallel computing.  
      
     Lastly, read section 10.1 of Chapter 10 on pages 207 and 208, which
    explains what R is.  
      
     The rest of the chapters of the text and the four appendices cover
    other interesting topics. These chapters and the appendices are
    optional.  
      
     Reading these chapters should take approximately 10 hours. Dedicate
    approximately 1 hour to 1.25 hours of study time to each chapter.
    Reading the optional chapters and appendices should take
    approximately 8 hours.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**The Saylor Foundation’s “Unit 8 Assessment”** <span id="8.5"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 8 Assessment: Parallel
    Processing”**
    Link: The Saylor Foundation’s [“Unit 8 Assessment: Parallel
    Processing”](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-8.FINAL_.pdf)
    (PDF)  
                  
     Instructions: Complete this assessment to test your knowledge of
    the concepts and learning outcomes for Unit 8. This assessment
    addresses the important topic of parallel processing as an approach
    for improving performance by using current building blocks. This
    topic involves both hardware and software and brings us back to the
    hardware/software interface that was introduced in Unit 1. Once you
    have completed the assessment, or if you need help, refer to the
    [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-8-Answer-Key.FINAL_.pdf).  
      
     Completing this assessment will take you approximately 2 hours.


