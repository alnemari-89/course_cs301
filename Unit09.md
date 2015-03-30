<<<<<<< HEAD
---
layout: default
title: "CS301: Computer Architecture"
course_description: "An exploration of the basic hardware/software components, assembly language, and functional architecture design of computers."
next: ../../../
previous: ../Unit08
---
=======
>>>>>>> master
**Unit 9: Look Back and Look Ahead** <span id="9"></span> 
*This unit looks back at important concepts of computer architecture
that were covered in this course and looks ahead at some additional
topics of interest. Computer architecture is both a depth and breadth
subject. It is an in depth subject that is of particular interest if you
are interested in computer architecture for a professional researcher,
designer, developer, tester, manager, manufacturer, etc. and you want to
continue with additional study in advanced computer architecture. On the
other hand, computer architecture is a rich source of ideas and
understanding for other areas of computer science, giving you a broad
and stronger foundation for the study of programming, computer
languages, compilers, software architecture, domain specific computing
(e.g., scientific computing), etc.*  
  
 *In this unit, you will look back at some of the theoretical laws and
analysis techniques that were introduced during the course. Looking
ahead, you will be introduced to special purpose processors, application
specific processing, high volume data storage, and network computing.*

**Unit 9 Time Advisory**  
Completing this unit should take approximately 8 hours.  
  
 ☐    Subunit 9.1: 2 hours  
  
 ☐    Subunit 9.2: 1 hour  
  
 ☐    Subunit 9.3: 5 hours

**Unit9 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   discuss basic laws applicable to computer performance;  
      
-   identify examples of computer architecture for special purpose
    computing architectures; and  
      
-   identify examples of special purpose applications of parallel
    computing.

**9.1 Theory and Laws** <span id="9.1"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 2: Parallel
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 2: Parallel
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read section 2.6 of Chapter 2 on pages 68 - 76 to
    learn about network topologies. If a task cannot be performed by a
    computer with one processor, we decompose the task into subtasks,
    which will be allocated to multiple hardware devices, say processors
    or arithmetic units or memory. These multiple hardware devices need
    to communicate so that the original task can be done with acceptable
    cost and performance. The hardware devices and their
    interconnections form a network.   
        
     Consider another situation: suppose we have a large software system
    made up of a large number of subsystems, in turn composed of many
    software components, subcomponents, etc. Suppose we list all the
    lowest level subcomponent’s names across the top of a sheet of
    paper. These will be our column headings. Also, let’s list down the
    side of the same sheet the same subcomponent names. These will be
    our row headings. This forms a table or two by two matrix. Finally,
    suppose we put a 1 in the table whenever or wherever there is a
    connection between the subcomponent named in the column heading and
    the subcomponent named in the row heading. Let’s put a 0 everywhere
    else. This table now represents a topology for our network of
    software components; it could also be done for hardware components.
    These components and their interconnections are part of the software
    architecture. Realize that the matrix could be huge: 100 by 100,
    1000 by 1000, etc. The complexity of the interconnections is a
    factor in the reliability and performance of the architecture.  
        
     Read section 2.7 of Chapter 2 on pages 77 - 79. This reading
    reviews Amdahl’s law, an extension of Amdahl’s law that includes
    communication overhead, and Gustafson’s law. These laws express
    expected performance as the number of processors increases, or as
    both the size of the problem and number of processors increases.  
     Then, read section 2.9 of Chapter 2 on pages 80 and 81 to learn
    about load balancing. This reading looks at the situation where a
    processor is idle and another is busy, which is referred to as a
    load imbalance. If the work were to be distributed differently among
    the processors, then the idle time might be able to be eliminated.
    This brief reading poses the load balance problem as a graph
    problem.  
        
     Reading these sections should take approximately 2 hours.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**9.2 Special Purpose Computing Architectures** <span id="9.2"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapter 2: Parallel
    Computer Architecture”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapter 2: Parallel
    Computer
    Architecture”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
      
     Instructions: Read section 2.8 of Chapter 2 on pages 79 and 80 to
    learn about GPU computing. GPU stands for Graphics Processing Unit.
    These are of interest because of the increase in the amount of
    graphics data handled by popular laptops and desktop computers.
    Furthermore, it turns out that since a GPU does primarily arithmetic
    computations, the architecture of a GPU is applicable to other types
    of applications that involve arithmetic on large amounts of data.  
      
     Read section 2.10 of Chapter 2 on pages 82 and 83 to learn about
    distributed, grid, and cloud computing. These are configurations of
    multiple computers for increasing performance and/or decreasing cost
    for high volume database access, sharing of resources, or accessing
    remote computer resources, respectively.  
        
     Reading these sections should take approximately 30 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

-   **Reading: Wikipedia: “TOP500”**
    Link: Wikipedia:
    [“TOP500”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-9.2-TOP500-Wikipediathefreeencyclopedia-CCBYNCSA_files/CS301-9.2-TOP500-Wikipediathefreeencyclopedia-CCBYNCSA.html) (HTML)  
      
     Instructions: Read this article, paying particular attention to the
    rankings of supercomputers, based on performance in running a
    LINPACK benchmark for computing a dense set of linear equations.
    Towards the end of the article, note the large number of cores in
    these supercomputers.  
        
     Reading this article should take approximately 30 minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/TOP500).

**9.3 Case Study: Special Purpose Applications of Parallel Computing**
<span id="9.3"></span> 
-   **Reading: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: “Chapters 4–8”**
    Link: Eijkhout, Chow, and van de Geijn’s *Introduction to
    High-Performance Scientific Computing*: [“Chapters
    4–8”](http://www.saylor.org/site/textbookuploads/5345_scicompbook.pdf) (PDF)  
        
     Instructions: Read Chapters 4–8, which describe problems pertaining
    to special application areas, called *domains*.  
        
     Reading these chapters should take approximately 5 hours.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/). It is
    attributed to Eijkhout, Chow, and van de Geijn, and the original
    version can be found
    [here](http://tacc-web.austin.utexas.edu/veijkhout/public_html/istc/istc.html).

**Final Exam** <span id="10"></span> 
-   **Final Exam: The Saylor Foundation’s “CS301 Final Exam”**
    Link: The Saylor Foundation’s [“CS301 Final
    Exam”](http://school.saylor.org/mod/quiz/view.php?id=893)  
      
     Instructions: You must be logged into your Saylor Foundation School
    account in order to access this exam. If you do not yet have an
    account, you will be able to create one, free of charge, after
    clicking on the link.


