# Do Serving Methods Affect Soda Enjoyment?
A Factorial Experiment with Regression Analysis

Factorial experiment analyzing how serving methods affect soda enjoyment.

---

## Project Overview

This project investigates whether serving conditions, specifically how soda is poured and consumed, affect perceived enjoyment.

While taste is typically attributed to ingredients, prior research suggests that presentation and consumption context may influence sensory perception. This study applies a controlled experimental design to test whether these factors meaningfully impact user experience.

---

## Research Question

Do serving methods significantly affect soda enjoyment?

Specifically:
- Does the pouring method influence enjoyment?
- Does the consumption method influence enjoyment?
- Is there an interaction effect between the two?

---

## Experimental Design

This study uses a 3 x 2 full factorial design with blocking:

Factor 1: Pouring Method (3 levels)
- Down the side of a glass  
- Straight into the center of a glass  
- Directly from the can  

Factor 2: Consumption Method (2 levels)
- Straw  
- Direct  

Blocking Variable:
- Participant (each participant tested all 6 conditions)

Each participant rated all treatment combinations on a 0 to 10 enjoyment scale, forming a within-subject design.

---

## Methodology

Model:
lm(score ~ pouring_method * consumption_method)

Key steps:
- Pilot study conducted to estimate variance and effect size  
- Power analysis performed to determine required sample size  
- Full experiment conducted with sufficient statistical power  
- Residual diagnostics performed:
  - Histogram  
  - Q-Q plot  
  - Residuals vs fitted  
- Permutation test applied due to non-normal residuals  

---

## Results

- No statistically significant effects were found:
  - Pouring method: not significant  
  - Consumption method: not significant  
  - Interaction effect: not significant  

- Enjoyment scores were consistently high across all conditions (mostly between 7 and 10)

---

## Key Insights

Despite common assumptions that serving conditions influence beverage experience:

Soda enjoyment appears largely invariant to serving method under controlled conditions.

Possible interpretations:
- Psychological expectations may outweigh physical differences  
- Effects may exist but are too small to detect with this sample size  
- Individual preference dominates treatment effects  

---

## Limitations

- Relatively small sample size  
- Limited variation in response scale (scores concentrated in 5 to 10 range)  
- Potential carbonation loss during sequential tasting  
- Within-subject fatigue or order effects  

---

## Key Takeaways

This project demonstrates:
- Experimental design (factorial with blocking)  
- Regression-based inference  
- Power analysis using pilot data  
- Model diagnostics and robustness checks  

It reflects a workflow similar to:
- A/B testing  
- Product experience analysis  
- Sensory evaluation studies  

---

## Project Structure

soda-experiment-analysis/
- README.md  
- analysis.Rmd  
- data/  
- plots/  

---

## Tools and Skills

- R / RStudio  
- Linear regression (lm)  
- Experimental design  
- Data visualization (ggplot2)  
- Statistical inference  
- Power analysis  
- Permutation testing  

---

## Future Improvements

- Increase sample size for higher statistical sensitivity  
- Introduce additional variables (temperature, carbonation level)  
- Improve experimental control (timing, serving consistency)  
- Explore mixed-effects models for participant-level variation  
