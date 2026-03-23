---
created: "2026-02-25 at 09:20"
tags:
  - fleeting
publish: "false"
---
W. Mei and Yaakov Bar-Shalom, “Unbiased Kalman filter using converted measurements: revisit,” _Proceedings of SPIE_, Aug. 2009, doi: https://doi.org/10.1117/12.831218.

---
## Motivation

> Why are they doing the work? Which problems are they trying to address.

- The authors found that existing unbiased converted measurement Kalman filters (CMKFs) can still produce biased estimates under certain conditions.
- Specifically, the covariance of the converted measurement is a noisy stochastic process that has a strong correlation with the measurement noise.
> What is the main purpose of conducting this particular research study?

- The purpose is to provide a new definition of unbiased measurement conversion, clearly distinguishing between a "measurement conversion without bias" and a "CMKF with an unbiased state estimate".
- The study aims to propose an efficient method to overcome the bias introduced by the correlation between the measurement covariance and measurement noise.
> What are the key research questions asked by the author(s)?

- While not explicitly phrased as a question, the core inquiry is: How can the filter gain of the CMKF be decorrelated from the measurement noise to ensure the weighted innovations remain zero mean and the filter remains unbiased?
## Approach of modelling

> What are the assumptions made and the limitations imposed by the authors? 

- For their proposed solution, they assume that the converted measurement noise covariance does not change significantly from time k to k+1 due to the geometry.
- To keep the theoretical discussion concise, their derivations are based on a 2-dimensional case, though simulations are expanded to a 3-dimensional scenario.
> What approach / model do they use as standard / baseline / reference?

- The authors use four existing measurement conversion methods as baselines: standard conversion, debiased conversion (1993), unbiased conversion (1998), and modified unbiased conversion (2004).

> What new approach / model do they propose, i.e. how is their approach different from the standard model?

- The authors propose the "Decorrelated CMKF" (DCMKF).
- Instead of using the converted measurement covariance at the current time step $(k+1)$ which introduces the problematic correlation—they propose using the measurement covariance from the previous time step $(k)$ to calculate the filter gain.
- This simple shift decorrelates the filter gain from the innovation, allowing the Kalman filter to give unbiased estimates with negligible performance loss.
## Approach of measuring Results and Benchmarking

> What are typical performance benchmarks, i.e. which parameters/variables are used to measure the success of the model implementation? Also identify possible intermediate variables that are sometimes measured directly in experiments, and then used to extract the final performance benchmark.

- The primary benchmarks are average measurement error, average estimation error, and Root Mean Square (RMS) position errors
- They also measure statistical consistency/unbiasedness using a calculated "3-sigma bound" (three times the standard deviation) for both measurement and estimation errors.

> What does the typical / standardised experiments entail to measure results?

- The experimental results are based on the average of 1000 Monte Carlo runs.
- The simulation features a 3-dimensional scenario where a fixed radar tracks a target over 100 scans with a 1-second sampling interval.
- The target's trajectory is generated using a second-order kinematic model that includes process noise.
> How are performance benchmarks derived from the experimental results?

- Performance benchmarks are derived by plotting the average measurement and estimation errors across the 100 scans and overlaying them with the 3-sigma bounds. If the errors stay within these bounds and center at zero, the estimates are considered unbiased.
- They also plot and compare the RMS position errors of their newly proposed DCMKF against the standard, unbiased, and modified unbiased CMKFs to evaluate overall tracking accuracy.
## Conclusion

> What did the authors ultimately achieve and conclude?

- The authors concluded that having unbiased converted measurements does not guarantee an unbiased state estimate because of the strong correlation between the measurement covariance and the measurement noise.
- They successfully demonstrated that their proposed Decorrelated CMKF (DCMKF) runs with no bias in all tested situations and provides the best RMS performance compared to the alternatives.
> Did they identify and outline limitations of their work and can we derive potential future research questions from these?

- While they did not outline explicit flaws in their proposed filter, they noted a potential area for future work: establishing a particle filter to compare its performance against the proposed CMKF.

