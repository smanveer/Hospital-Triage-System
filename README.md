HospitalTriageSystem

Implementing a system to triage patients in hospital emergency ward. 
Patients triaged according to:
--> Medical priority 
--> Wait time. 
Priorities are positive integers; the highest priority is 1. Normally patients are seen in priority order. However, if there are patients who have waited longer than a specified time (maxWait), they are seen first, in order of their arrival.

Adding and removing patient from the system is done in linear time.

Implementation:- To achieve this, the system uses two location-aware priority queues implemented with min heaps: one based on medical priority and the other on arrival time. The heaps use ArrayLists to store the underlying binary trees.
