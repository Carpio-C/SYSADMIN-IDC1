+----------------------------------+------------------------+----------+
| ![](vertopal_                    |                        |          |
| d174b7bee64f41a088f468f0ee2cc4e2 |                        |          |
| /media/image1.png){width="2.4in" |                        |          |
| height="0.5881944444444445in"}   |                        |          |
|                                  |                        |          |
| SCHOOL OF INFORMATION AND        |                        |          |
| TECHNOLOGY                       |                        |          |
+----------------------------------+------------------------+----------+
| NAME: Carpio, Charlimagne, V.    | DATE PERFORMED:        | /50      |
|                                  |                        |          |
| Pacio, Dee Jay, T.               |                        |          |
+----------------------------------+------------------------+----------+
| Section:IDC1                     | DATE SUBMITTED:12/3/24 |          |
+----------------------------------+------------------------+----------+

# SYSADM1 -- Capacity Management & Planning

**Part 2. Network Scalability Analysis**

Recall the e-commerce website scenario we discussed earlier. Given the
expected surge in traffic, analyze the provided network topology
diagram. Identify potential bottlenecks and areas where scalability
might be a concern. Propose specific strategies to improve the
network\'s scalability and performance to ensure a seamless user
experience during the peak traffic period. Consider factors such as
increased user demand, new applications, and security threats.

![](vertopal_d174b7bee64f41a088f468f0ee2cc4e2/media/image2.bin){width="5.049483814523184in"
height="3.8229166666666665in"}

Potential Bottlenecks:

Edge Router Capacity- A single edge router processes all incoming and
outgoing traffic. During peak traffic, this may lead to network
slowdowns, dropped connections, and downtime if the router fails.

Core Switch- No redundancy, the entire network could fail if this switch
becomes unresponsive.

VLAN's - Imbalanced traffic and underutilized resources across VLANs.

No security measure- making the network vulnerable to external threats.

Proposed Strategies:

-   We added 1 more core router so that the network can handle more
    traffic and provides availability. Also, if one router fails, the
    other router takes over seamlessly.

-   We also added 1 more core switch for enhanced scalability,
    redundancy, and faster inter-VLAN communication.

-   Load balancers were implemented within each VLAN to ensure even
    distribution of incoming traffic.

-   Added firewall with IDS/IPS to monitor all incoming and outgoing
    traffic, filters malicious requests, and mitigates potential threats
    in real-time.

-   We also added a monitoring system to track real-time performance
    metrics, detect anomalies, and provide alerts for security threats

Diagram:

![Diagram](https://github.com/Carpio-C/SYSADMIN-IDC1/blob/1a3a0e71273bcc8329db07ffe25d44985fbd2e82/Images/Diagram.png)

  ------------------------------------------------------------------------------
  Criteria          Excellent \| 10pts Good \| 7pts        Needs Improvement \|
                                                           4pts
  ----------------- ------------------ ------------------- ---------------------
  **Network         Accurately         Identifies key      Identifies some basic
  Analysis**        identifies         network components  network components
                    potential          and some potential  but lacks a
                    bottlenecks,       bottlenecks.        comprehensive
                    security risks,                        analysis.
                    and capacity                           
                    limitations.                           

  **Scalability     Proposes multiple  Proposes some       Proposes limited
  Planning**        relevant solutions relevant            scalability
                    and provides       scalability         strategies.
                    detailed           strategies but      
                    explanations,      lacks detail.       
                    including                              
                    potential                              
                    drawbacks and                          
                    benefits.                              

  **Evaluation of   Proposes           Provides a basic    Does not evaluate the
  Solutions**       comprehensive      evaluation of the   proposed solutions or
                    scalability        proposed solutions, provides a
                    strategies,        but lacks depth.    superficial
                    including specific                     evaluation.
                    recommendations                        
                    for hardware                           
                    upgrades, software                     
                    configurations,                        
                    and network                            
                    optimizations.                         

  **Proposed        Provides a         Provides a basic    Does not provide a
  Design**          detailed and       design but lacks    clear and detailed
                    well-justified     specific details    design.
                    design, including  and justifications. 
                    network diagrams,                      
                    configuration                          
                    details and                           
                    implementation                         
                    plans.                                 

  **Evaluation and  Provides a         Provides a basic    Does not evaluate the
  Justification**   thorough           evaluation of the   proposed solutions or
                    evaluation of the  proposed solutions, provides a
                    proposed           but lacks depth.    superficial
                    solutions,                             evaluation
                    considering                            
                    factors like cost,                     
                    complexity, and                        
                    potential impact.                      

  Score:                                                   /50
  ------------------------------------------------------------------------------
