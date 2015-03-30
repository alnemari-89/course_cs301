<<<<<<< HEAD
---
layout: default
title: "CS301: Computer Architecture"
course_description: "An exploration of the basic hardware/software components, assembly language, and functional architecture design of computers."
next: ../Unit07
previous: ../Unit05
---
=======
>>>>>>> master
**Unit 6: The Memory Hierarchy** <span id="6"></span> 
*In prior units, you have studied elementary hardware components, e.g.,
combinational circuits and sequential circuits; functional hardware
components, such as adders, arithmetic logical units, data buses; and
computational components, such as processors.*  
  
 *This unit will address the memory hierarchy of a computer and will
identify different types of memory and how they interact with one
another. This unit will look into a memory type known as* *cache and
will discuss how caches improve computer performance. This unit will
then discuss the main memory, DRAM (or the Dynamic Random Access
Memory), and the associated concept of virtual memory. You will take a
look at the common framework for memory hierarchy. The unit concludes
with a review of the design of a cache hierarchy for an industrial
microprocessor.*

**Unit 6 Time Advisory**  
Completing this unit should take approximately 10.75 hours.  
  
 ☐    Subunit 6.1: 2.5 hours  
  
 ☐    Subunit 6.2: 2.5 hours  
  
 ☐    Subunit 6.3: 1.25 hours  
  
 ☐    Subunit 6.4: 2.5 hours  
  
 ☐    Unit 6 Assessment: 2 hours

**Unit6 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   explain the importance of memory hierarchy in computer design, and
    explain how memory design impacts overall hardware performance.

**6.1 Elements of Memory Hierarchy and Caches** <span id="6.1"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Memory Hierarchy: Basic Idea”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Memory Hierarchy: Basic
    Idea”](http://www.youtube.com/watch?v=_eAL-v5oNOw) (YouTube)  
        
     Instructions: Watch the video lecture. Previously, you have focused
    on processor design to increase performance. Now, you will turn to
    memory. This video introduces various methods of improving processor
    performance through the use of memory hierarchy. The lecture
    discusses memory technologies, which vary in cost and speed. We have
    to assume that memory is flat, but with current technology, flat
    memory does not meet performance demands placed on it. You will take
    a look at hierarchical memory and the use of cache. This video will
    also discuss analysis of memory hierarchies and cache performance
    with respect to miss rates and block size. Finally, the lecturer
    considers cache policy.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1 hour and 30 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 1: Sequential
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 1: Sequential
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read section 1.2 of Chapter 1 on pages 14–23 to learn
    about memory hierarchies, and read section 1.4 on pages 25–29 to
    learn about locality and data reuse. Subsections 1.2.6 and 1.2.7
    apply to the topics outlined below in subunits 6.2 and 6.3. These
    readings supplement the memory topics discussed in Kumar’s video.  
        
     Reading these sections should take approximately 1 hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**6.2 Cache Architectures and Improving Cache Performance** <span
id="6.2"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Memory Hierarchy: Cache Organization”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Memory Hierarchy: Cache
    Organization”](http://www.youtube.com/watch?v=6F6NP1lrRpc&feature=relmfu) (YouTube)  
      
     Instructions: Watch this lecture on memory hierarchy design with
    caches. This lecture discusses the impact that memory operations
    have on overall processor performance and identifies different cache
    architectures that can improve overall processor performance. In the
    memory hierarchy, from top to bottom, there are:

    -   processor registers,
    -   cache,
    -   main memory, and
    -   secondary memory.

    The order goes from faster, smaller capacity, and higher cost to
    slower, higher capacity, and lower cost. Data moves from the main
    memory to cache. To do this requires a mapping from addresses in the
    main memory to cache addresses. How this is done affects
    performance. Performance analysis of cache and memory organization
    involves miss rate and miss penalty. Policies for reading, loading,
    fetching, replacing, and writing memory also affect cost and
    performance.  
      
     Watching this lecture and pausing to take notes should take
    approximately 1 hour and 30 minutes.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 1: Sequential
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 1: Sequential
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read section 1.5 of Chapter 1 on pages 30–41. This
    reading discusses the relationship of pipelining and cache to
    programming.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**6.3 Main Memory and Virtual Memory** <span id="6.3"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “Memory Hierarchy: Virtual Memory”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“Memory Hierarchy: Virtual
    Memory”](http://www.youtube.com/watch?v=cIlKSD8ptAk) (YouTube)  
      
     Instructions: Watch this lecture, which addresses the subject of
    virtual memory. This topic pertains to the relationship of main
    memory and secondary memory and has similarities and differences to
    the relationship of cache and main memory. Differences arise due to
    the speed of the various memories and their capacities. This lecture
    discusses virtual memory, mapping from virtual memory addresses to
    physical addresses in main and paging techniques used with the main
    memory. The lecture discusses the use of page tables in translating
    virtual addresses to physical addresses. Issues that arise with page
    tables include structure, location, and large size.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1.25 hours.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**6.4 Performance Tuning** <span id="6.4"></span> 
-   **Reading: Lawrence Livermore National Laboratory: Blaise Barney’s
    *Introduction to Parallel Computing*: “Chapters 1–5”**
    Link: Lawrence Livermore National Laboratory: Blaise Barney’s
    *Introduction to Parallel Computing*: [“Chapters
    1–5”](https://computing.llnl.gov/tutorials/parallel_comp/#DesignCosts) (HTML)  
        
     Instructions: Read Chapters 1–5. Before reading these chapters,
    list the factors that you can think of that can affect performance,
    e.g., memory performance, cache, memory hierarchy, multi-cores, etc.
    and what you might suggest as ways to increase performance. After
    reading these chapters, what might you add, if anything, to your
    list?  
        
     Reading these chapters, creating the list of factors, and taking
    notes should take approximately 2.5 hours.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above. 

**The Saylor Foundation’s “Unit 6 Assessment”** <span id="6.5"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 6 Assessment: Memory
    Hierarchy”**
    Link: The Saylor Foundation’s [“Unit 6 Assessment: Memory
    Hierarchy”](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-6.FINAL_.pdf)
    (PDF)  
                  
     Instructions: Complete this assessment to test your knowledge of
    the concepts and learning outcomes for Unit 6. This assessment
    requires you to take a closer look at one of the most limiting, with
    respect to overall performance, of our building block components,
    namely, memory. Once you have completed the assessment, or if you
    need help, refer to the [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-6-Answer-Key.FINAL_.pdf).  
      
     Completing this assessment will take you approximately 2 hours.


