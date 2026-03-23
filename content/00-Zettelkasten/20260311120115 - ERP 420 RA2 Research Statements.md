---
created: "2026-03-11 at 12:01"
tags:
  - fleeting
publish: "false"
---
> Searching for an interesting research question
---
- Our research project is interested in investigating statistical sensor fusion algorithms for Cartesian coordinate object tracking with polar measurements. However, polar measurements have limitations such as nonlinearities, susceptibility to noise and individual inaccuracies.
- So our system is successful if we can estimate an object's state through application of a statistical sensor fusion algorithm that processes the polar measurements **and** if a toolset can perform a statistical analysis of the generated data.
- Limitations for the research project implementation:
	- Restricted to the statistical approach at a software level when performing object state space estimation.
	- If my idea is novel or ventures into the unknown, it would be recommended to discuss this with the lecturer.

> [!NOTE] How to get started
> I feel that we need to restate the objective of our research and then consider what was done by papers in RA1 again.

- Our most recent paper from RA1, [[20260225201725 - Drafting ERP 420 RA1]] saw us look at [[20260225193133 - Decorrelated Unbiased Converted Measurement Kalman Filter]].
- In practical 1, several tasks are highlighted.
	- The first is interested in how the object is modeled. Can consider whether the object dynamics model can be manuevering or non-maneuvering.
	- The second is interested in sensors that provide range and bearing data such as RADAR, SONAR, LIDAR.
	- But Task C is the money. The non linearities of converting between state space affect the estimation, filtering and uncertainty propagation. 
- 