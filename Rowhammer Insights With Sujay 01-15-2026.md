# Short interview with Sujay Yadalam Sudarshan. 01-15-2026 (raw notes)

Previous researcher at Microsoft. Rowhammer attacks at the architectural level. PhD in Computer Science at University of Wisconsin-Madison. 

## 1.	ASKING ABOUT HIS RESEARCH EXPERIENCE
-	At a high level, what was the focus of your Rowhammer work at Microsoft—was it primarily experimental characterization, mitigation design, or security exploitation?
Characterization and mitigation, implemented in memory controller and structure to metadata to prevent rowhammer 
DRAM rowhammer window threshold, if i accesss it so many time prob of bit flip is high. 
Make sure that treat reaching the threshold as the attack. never allow row to be activated x amount of times. 

-	How much of the work was exploratory research versus engineering mitigation for production systems?
started as a research project, working with architectural team. having many constraints from hardware team, while developing architecture

## 2.	GOAL 1: SIMULATE A ROWHAMMER ATTACK AT THE PHYSICAL LEVEL
-	From your experience, which physical mechanisms dominate Rowhammer-induced bit flips: charge leakage, capacitive coupling, sense amplifier disturbance, or something else?
speculative: coupling main issue, charge leak was not the main. coupling was row to cell not row to cell.

-	If you were building a Rowhammer simulation today, what abstractions would you keep and what would you avoid?

simulators onur mukryu (the prof from Europe) ramulator
have to know how many access between two activates in a row. 

-	In your view, why has industry largely favored mitigation techniques (e.g., TRR, refresh rate increases) instead of architectural/physical elimination?

fixing takes time, fundamental changes to dram design, though gap solution (used today)
ram works with very small margins. would make cost levels high. 

## 3.	RESEARCH
-	Which papers or authors other than prof. mutlu were most influential in your work?
Stefan Saroiu, Moinuddin K. Qureshi
https://moin.cc.gatech.edu/
https://stefan.t8k2.com/


## 4.	CONCERNS
-	Given my goal to simulate Rowhammer at the physical level and redesign DRAM to eliminate it, where do you see the biggest risk of over-simplification?
Main challenge is to characterize the failure itself, since its all mostly theory at the moment. Not a single case of rowhammer attacks 



## 5.	RESEARCH SOURCES:
1) DRAM SEC
2) Start with Revisiting RowHammer: https://arxiv.org/abs/2005.13121
3) Graphene: Strong yet Lightweight Row Hammer Protection: https://ieeexplore.ieee.org/abstract/document/9251863
--> Search with connected papers: https://www.connectedpapers.com/

## 6.	MISC
-	Mitigation techniques: 
Per Row Activation Counting (PRAC)

-	ROWHAMMER SIMULATION TOOLS:
https://github.com/CMU-SAFARI/ramulator
https://github.com/CMU-SAFARI/ramulator2
-	Micron Connections
https://www.linkedin.com/in/jeremy-chritz-58008215/
https://www.linkedin.com/in/randall-rooney-399546b/
-	Misc Connections
Prashant Nair
UBC Quantum Computing 
https://ece.ubc.ca/prashant-nair/





