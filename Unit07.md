---
layout: default
title: "CS301: Computer Architecture"
course_description: "An exploration of the basic hardware/software components, assembly language, and functional architecture design of computers."
next: ../Unit08
previous: ../Unit06
---
**Unit 7: Storage and I/O** <span id="7"></span> 
*In this unit, we will discuss the input/output devices that enable
communication between computers and the outside world in some form. The
reliability of these devices is important; we will accordingly discuss
the related issues of dependability, availability, and reliability. You
will also take a look at non-volatile storage mediums, such as* *disk
and flash memory, before learning about mechanisms used to connect the
computer to input/output devices. This unit will conclude by discussing
disk system performance measures.*

**Unit 7 Time Advisory**  
Completing this unit should take approximately 6.75 hours.  
  
 ☐    Subunit 7.1: 1.5 hours  
  
 ☐    Subunit 7.2: 1.5 hours  
  
 ☐    Subunit 7.3: 1 hour  
  
 ☐    Subunit 7.4: 0.75 hours  
  
 ☐    Unit 7 Assessment: 2 hours

**Unit7 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:  
-   discuss storage and I/O devices, their performance measurement, and
    RAID technology.

**7.1 I/O Devices** <span id="7.1"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “I/O Subsystem: Introduction”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“I/O Subsystem:
    Introduction”](http://www.youtube.com/watch?v=0XybwAbup-w) (YouTube)  
      
     Instructions: Watch this lecture, which discusses the basic ideas
    behind the input/output (I/O) subsystem of a computer system. The
    lecturer also looks into performance measurement for I/O devices and
    interfaces used to interconnect I/O devices to the processor. This
    is the first of two video lectures on I/O. A computer subsystem
    consists of three major components: processor, memory, and
    connections. The key words in the previous sentence aresubsystemand
    connections. To be useful, a computer system needs to have
    connections with external devices to get data and control signals
    into the computer and to put data and control signals out. The
    external devices can be other systems or other systems may be
    connected to the same devices. Thus, our computer system is part of
    a network of a few or many other subsystems interconnected to
    perform useful tasks.  
      
     We are always interested in how well a task is performed, in terms
    of time, capacity, and cost. In considering performance relative to
    our useful task, we have to consider processor performance, memory
    performance, and the performance of the connections, including the
    performance of the external devices. This first video lecture looks
    at external or peripheral devices and I/O performance. The next
    video in subunit 7.2 discusses interfaces, buses, and I/O
    transfer.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1 hour and 30 minutes.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**7.2 Connecting I/O Devices to the Processor** <span id="7.2"></span> 
-   **Lecture: YouTube: Indian Institute of Technology, Delhi: Anshul
    Kumar’s “I/O Subsystem: Interfaces and Buses”**
    Link: YouTube: Indian Institute of Technology, Delhi: Anshul Kumar’s
    [“I/O Subsystem: Interfaces and
    Buses”](http://www.youtube.com/watch?v=myVbSSyZtr4) (YouTube)  
      
     Instructions: Watch this lecture for an introduction to the
    interconnection schemes used for the input/output (I/O) subsystem of
    a computer system. This is the second of two lectures on I/O
    devices. The previous lecture looked at the connection of memory,
    either cache or main memory, with peripheral devices and the
    transfer and transformation of data between them. This video lecture
    analyzes alternative interconnection schemes with a focus on buses.
    Also, it discusses protocols for the data that flows on the buses:
    asynchronous and synchronous. A *synchronous protocol*uses a clock
    to time sequence the information flow. An *asynchronous
    protocol*does not use a clock; the signal carries the sequencing
    information. Then, the lecture shows a performance comparison of two
    different protocols.  
        
     Watching this lecture and pausing to take notes should take
    approximately 1 hour and 30 minutes.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-NoDerivs 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-nd/3.0/).

**7.3 Measuring Disk Performance** <span id="7.3"></span> 
-   **Reading: Wikipedia: “Hard Disk Drive Performance
    Characteristics”**
    Link: Wikipedia: [“Hard Disk Drive Performance
    Characteristics”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-7.3-Harddiskdriveperformancecharacteristics-Wikipediathefreeencyclopedia-CCBYNCSA_files/CS301-7.3-Harddiskdriveperformancecharacteristics-Wikipediathefreeencyclopedia-CCBYNCSA.html) (HTML)  
        
     Instructions: Read this article. Disks have various
    characteristics, which determine quality attributes, such as
    reliability, performance, etc. Here, we are interested in
    performance. Think of some characteristics that affect performance.
    How can performance of a disk be measured?  
        
     Reading this article should take approximately 1 hour.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/Disk-drive_performance_characteristics).

**7.4 Redundant Array of Inexpensive Disks (RAID)** <span
id="7.4"></span> 
-   **Reading: DBpedias: “Understanding Storage Technology – RAID
    Technology”**
    Link: DBpedias: [“Understanding Storage Technology – RAID
    Technology”](http://dbpedias.com/wiki/Oracle:Understanding_Storage_Technology#RAID_Technology)
    (HTML)  
      
     Instructions: Read the “RAID Technology” section, stopping at
    “Storage Area Networks,” to learn about RAID storage. This reading
    introduces the commercial technology for disk reliability, one of
    the quality attributes important for data storage devices.   
      
     Reading this section and taking notes should take approximately 15
    minutes.  
        
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-NonCommercial-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-nc-sa/3.0/). You can
    find the original DBpedias version of this
    article [here](http://dbpedias.com/wiki/Oracle:Understanding_Storage_Technology#RAID_Technology).

-   **Reading: Wikipedia: “RAID”**
    Link: Wikipedia:
    [“RAID”](http://resources.saylor.org.s3.amazonaws.com/CS/CS301/CS301-7.4-RAID-Wikipediathefreeencyclopedia-CCBYNCSA_files/CS301-7.4-RAID-Wikipediathefreeencyclopedia-CCBYNCSA.html) (HTML)  
      
     Instructions: Read the following sections of this article: Standard
    Levels, RAID Parity, New RAID Classification, Reliability Terms, and
    Problems with RAID. This reading will provide you with a description
    of RAID technology and will introduce you to techniques that are
    used for studying performance and reliability in general.  
      
     Reading these sections should take approximately 30 minutes.  
      
     Terms of Use: This resource is licensed under a [Creative Commons
    Attribution-ShareAlike 3.0 Unported
    License](http://creativecommons.org/licenses/by-sa/3.0/). You can
    find the original Wikipedia version of this
    article [here](http://en.wikipedia.org/wiki/RAID).

**The Saylor Foundation’s “Unit 7 Assessment”** <span id="7.5"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 7 Assessment: Storage
    and I/O”**
    Link: The Saylor Foundation’s [“Unit 7 Assessment: Storage and
    I/O”](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-7.FINAL_.pdf)
    (PDF)  
                  
     Instructions: Complete this assessment to test your knowledge of
    the concepts and learning outcomes of Unit 7. This assessment
    focuses on the building block components for input and output. These
    I/O components have evolved significantly over the last 50 years.
    Therefore, we can expect there will be significant development of
    I/O devices in coming years, as computing applications expand more
    into our everyday lives. Once you have completed the assessment, or
    if you need help, refer to the [Answer
    Key](http://www.saylor.org/site/wp-content/uploads/2012/08/CS301-Computer-Architecture-Assessment-7-Answer-Key-FINAL.pdf).  
      
     Completing this assessment should take approximately 2 hours.


