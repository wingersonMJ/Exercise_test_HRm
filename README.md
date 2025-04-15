# Predicting exercise test performance in adolescents with concussion
Wingerson, MJ  
mat.wingerson@gmail.com

# Description 
Transparency of source code and results for a manuscript submitted to [journal tbd]. 

[Add citation when accepted]

---

# Overview

## Background:
Engaging in aerobic exercise within days of concussion is the standard of care treatment approach [[ref](https://pubmed.ncbi.nlm.nih.gov/37316185/)]. While the precise dosage of exercise that is optimal for treatment of post-concussion symptoms and other impairments remains a popular research topic, consensus has generally been reached that exercise at an intensity, duration, and frequency that does not exacerbate symptoms is considered safe and beneficial for recovery [[ref](https://pubmed.ncbi.nlm.nih.gov/37316210/), [ref](https://pubmed.ncbi.nlm.nih.gov/30715132/)].  

A common practice for prescribing exercise in clinical settings is through the use of an exercise test [[ref](https://pubmed.ncbi.nlm.nih.gov/40135995/)]. In the controlled clinical setting, a graded exercise test can gradually increase heart rate from resting to moderate/high intensity over the course of 10-15 minutes. Clinicians can monitor patients during the test, looking for one of two stopping criteria: a) an increase in symptoms that is more than mild, b) reaching the point of self-reported exhaustion (typically reported through a percieved exertion scale), or a heart rate that approaches the patients age-predicted maximum heart rate (220bmp - age, HRm), also considered exhaution. Uppon reaching a stopping criteria, clinicians can measure the highest heart rate achieved on the test, refered to as the symptom threshold, or the maximum heart rate the patient is able to tolerate before symptoms increase or exhaustion is reached. The clinician is then able to prescribe 80-90% of this highest heart rate as the heart rate target (HRt), which provides a patient-specific exercise recomendation to perform as part of their recovery. Past work has shown that a HRt of 90% of the highest achieved heart rate during testing for 20-30 minutes, 4-5 days per week is safe and effacous for recovery [[ref](https://pubmed.ncbi.nlm.nih.gov/35489100/) - our work!].  

## Knowledge Gaps:
Though exercise testing for the purposes of deriving patient-specific HRt's is standard clinical practice, no research has systematically described performance during exercise testing with respect to the progression of patient heart rate, rating of percieved exertion, or symptom exacerbation. Demographic, injury, and clinical factors associated with the stopping criteria, or the highest heart rate achieved on the test, have also not been investigated.

Last, though exercise testing is ideal for developing personalized HRt prescriptions for adolescents after concussion, alternative methods exist for deriving heart rate prescriptions in the abscence of exercise tests. One such example is to prescribe 50% of the patients age-predicted maximum heart rate (220bpm - age, HRm). However, this recommendation is an approximation of what it is believed patients will achieve if they had recieved an exercise test, and the actual value ranges from 50-80% of HRm, a wide range that lacks evidential support. 

## Objective:
1. To compare demographics, injury, and clinical characteristics among participants with concussion based on exercise test stop criteria: symptom exacerbation vs exhaustion.

2. To determine if demographics, injury, or clinical characteristics are associated with the maximum achieved heart rate on the exercise test.

3. To evaluate the accuracy of a 50% HRm method for prescirbing a HRt compared to the HRt derived from exercise testing. 

---

# Methods

## Exercise testing:
The graded YMCA protocol is described in our past exercise RCT [[ref](https://pubmed.ncbi.nlm.nih.gov/35489100/) - our work!]. It is similar to the Buffalo Concussion Test described here, but has some important differences that you will see [[ref](https://pubmed.ncbi.nlm.nih.gov/40135995/)]. Big picture summary: The test begins with a baseline measure of resting heart rate, then progresses through stages of exercise on a stationary bike for ~15 minutes. The beginning stages are low rpm (revolutions per minute) and low resistance (Watts). Every 2-3 minutes the rpms and resistance are increased to evoke a heart rate response (increase). The test is over when all stages are completed, or when one of two stop critera are met: 1) symptoms increase more than mildly, or 2) exhaustion is reached. A symptom increase of more than mild is defined as >3.0 points on a 10-point Visual Analog Scale (VAS), where 0.0 represents no symptoms and 10.0 represent the worst symptoms you can have. Exhaustion is defined as >= 17-points on the Borg's Rating of Percieved Exertion (RPE), where 6 represents resting effort and 20 represent the most effort a participant could give (17 generally equated to working "Very Hard"). Exhaustion could also be met if the participant reaches their age-predicted maximum heart rate (220bpm - age). The test can also be stopped if the pariticpant completes all stages, totally approximately 15 minutes of exercise. The highest heart rate achieved during the test is then multiplied by 0.90 (90%) to obtain the heart rate target (HRt). 

For the purposes of analysis, we grouped participants as having symptom exacerbation during the test vs reaching exhaustion/completing the protocol. 

## HRm Method:
Though exercise testing is ideal for developing personalized HRt prescriptions for adolescents after concussion, exercise testing can be burdensome (time, resource, and expertise demands). Therefore, past research has established alternative methods for generating heart rate prescriptions for patients in the abscense of exercise testing [[ref](https://pubmed.ncbi.nlm.nih.gov/32058454/)]. One approach established in previous work is to prescribe a portion of the patients age-predicted maximum heart rate (HRm). It has been suggested that 50% of HRm is recommended for patients as a starting point for exercise, progressing by +5% every day as symptoms allow up to a maximum of 80% HRm. 

**Definitions:**
HRt = Heart rate target, 90% of the highest heart rate achieved on exercise testing.
HRm = Heart rate max, calculated as 220bpm minus the participants age (i.e., 205bpm if age == 15years).

---

# Findings and Figures

## Pre-processing:
**Figure A (not for text):** Kernel density plot showing the distribution of the highest heart rate achieved on the exercise test in our sample. N=105
<img src="figs/pre-processing_kernelDensity.png" alt="KD pre-processing" width="1000">  
*Interpretation:* A majority of subjects reached a heart rate of between 150bpm and 200bpm during the test. Almost no one went above 200bpm and a smaller portion of the sample was between 100 and 150bpm. 
**Important on this plot is the small 'bump' at ~75bpm. N=4 subjects had a highest achieved heart rate of between 72 and 90bpm. These values are closer to what we would expect for a resting heart rate, not an ending heart rate. These points likely reflect an error in the data. Therefore, they were removed from the analysis.**

**Figure B (not for text):** Kernel density plot showing the distribution of the highest heart rate achieved on the exercise test in our sample. N=101
<img src="figs/post-processing_kernelDensity.png" alt="KD post-processing" width="1000">  
*Interpretation:* This is the same density plot as above, but with the N=4 outlier subjects removed. 

## Exercise test performance:
**Figure 1:** Changes in heart rate, symptoms (visual analog scale), and rating of percieved exertion throughout the exercise test. Mean values at each minute were calculated and ploted for those who stopped due to symptom exacerbation vs those who reached exhaustion or completed the protocol. 
<img src="figs/Figure1.png" alt="exercise test performance" width="1000">  
*Interpretation:* No significant differences in the heart rate achieved during the test, or in the progression of heart rate throughout the test, between those who stopped due to symptoms and those who reached exhaustion or completed the protocol. 

**Table A (can probably just describe this in the results, don't need to include this table):** Performance on the exercise test. 
|                                  |      | Missing   | Overall        | Range       |
|----------------------------------|------|-----------|----------------|-------------|
| n                                |      |           | 101            |             |
| branch_used, n (%)               | Easy |           | 78 (77.23)     |             |
|                                  |Medium|           | 18 (17.82)     |             |
|                                  | Hard |           | 3 (2.97)       |             |
| Fatigue, n (%)                   | 1    |           | 11 (10.89)     |             |
| Pain, n (%)                      | 1    |           | 1 (0.99)       |             |
| Diziness, n (%)                  | 1    |           | 22 (21.78)     |             |
| Headache, n (%)                  | 1    |           | 42 (41.58)     |             |
| Nausea, n (%)                    | 1    |           | 8 (7.92)       |             |
| highest_hr_achieved, mean (SD)   |      | 0         | 171.32 (17.57) |             |
| highest_rpe_achieved, mean (SD)  |      | 0         | 15.50 (2.32)   |             |
| highest_rpm_achieved, mean (SD)  |      | 1         | 73.05 (6.25)   |             |
| highest_vas_achieved, mean (SD)  |      | 1         | 3.76 (2.15)    |             |
| hr_baseline, mean (SD)           |      | 2         | 82.74 (12.02)  |             |
| vas_baseline, mean (SD)          |      | 2         | 1.98 (1.65)    |             |



## Factors associated with stop criteria:



## Factors associated with exercise test HRt:

## HRm performance metrics:

## Optimal HRm methods:

## Personalized prescription in the absence of exercise testing:





--- 

# Key take-aways
