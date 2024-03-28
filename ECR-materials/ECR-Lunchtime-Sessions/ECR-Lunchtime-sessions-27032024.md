# ECR Lunchtime sessions 2024
## AI for Multiple Long-term Conditions - Research Support Facility

:date: 27 March 2024 at 12.15 to 13.00 UTC

# The causes of multimorbidity?
## Speaker - Anthony Webster, Postdoctoral Statistician, Department of Statistics, University of Oxford.
**Details:** 
The talk will summarise several recent studies of UK Biobank data[1-5], from the perspective of multimorbidity. Their results emphasised the strength of associations between established risk factors and increased disease-risk, for many different diseases. They also suggested that most disease-risk might be explained by age and established risk factors alone, with the observed number of cases of order 50% greater than expected in otherwise disease-free individuals.

[1] “How much disease-risk is due to old age and established risk factors?”, A.J. Webster, PNAS Nexus, 2, 9, pgad279 (2023).

[2] "Causal attribution fractions, and the attribution of smoking and BMI to the landscape of disease incidence in UK Biobank", A.J. Webster, Scientific Reports 12, 19678 (2022).

[3] "Sporadic, late-onset, and multistage diseases", A.J. Webster, R. Clarke, PNAS Nexus, 1, 3, pgac095 (2022).

[4] "Characterisation, identification, clustering, and classification of disease", A.J. Webster, K. Gaitskell, I. Turnbull, B.J. Cairns & R. Clarke, Scientific Reports, 11, 5405 (2021).

[5] "Multi-stage models for the failure of complex systems, cascading disasters, and the onset of disease", A.J. Webster, PLOS One, 14 (5), e0216422 (2019).

### :clipboard: Roll call

> **Please put in your name, pronouns (if you like) affiliation & role.** 

> Please note that this document will be stored in a private GitHub repository used by the AIM RSF and AIM Consortia. By registering you acknowldge the [Turing Institute's Privacy Policy](https://www.turing.ac.uk/privacy-policy). You have the option of having your information withheld from the repository by adding the :shushing_face: emoji in front of your name. 

* Batool Almarzouq (she/her), Alan Turing Institute, Research Project Manager from Computational biology background
* Anthony Webster (anthony.webster@stats.ox.ac.uk), Statistician/Epidemiologist, Department of Statistics, University of Oxford.
* Paola Galdi (she/her), University of Edinburgh, Postdoctoral researcher, machine learning background
* Layik Hama (he/him), School of Computing, University of Leeds. Part of DynAIRx project.
* Sian Holt (she/her), University of Southampton, Research Fellow
* Guillermo Romero Moreno (he/him), University of Edinburgh, Research Associate based in Informatics
* Marco Canducci (he/him), University of Birmingham, School of Computer Science, Research Fellow
* Maurice O'Connell, The University of Manchester
* Louise Coutts, University of Southampton
* Alish Angdembe, QMUL
* Lizzie Remfry (she/her), QMUL
* Mozhdeh
* Rafael Henkin
* Sian
* Yu Liu
* Ellie Hathaway, University of Birmingham.
* Muhammed Usman, University of St-Andrews
* Daniel Phillips, University of Oxford

## Agenda

1. Welcome and ice breaker
2. Talk by Anthony Webster on The causes of multimorbidity? 
3. Discussion
4. AOB

## Ice breaker

**ICE BREAKER QUESTION - What is your most used emoji?**
You can use emoji copy to add it below - https://emojicopy.com/
* I'm currently in the Easter spirit 🐰 🥚 and thrilled about spending the next 2 weeks in AL!
* By far my most used emoji 😅 +1
* I am also on team laughing emoji 😂
* I go many times with an old-school : P
* thumbs up


## Notes

The talk titled "The Causes of Multimorbidity", was presented by Anthony Webster. It described findings from his 3-year fellowship project funded by the Nuffield Department of Population Health at the University of Oxford. The project's original focus was on characterising and classifying diseases, but many of the findings were relevant to multimorbidity. The study used data from the UK Biobank dataset.  

### Key points:

- Traditional epidemiological studies usually consider the risk of a single disease, in otherwise healthy individuals, and will typically exclude anyone with conditions that could potentially alter disease risk.
- This contrasts with clinical reality, where patients often have numerous co-existing diseases and pre-existing conditions (multimorbidity).
- He sought to analyse how many new disease onsets would be expected based solely on age and well-established risk factors like smoking, assuming individuals were healthy at baseline.
- His results showed a surprisingly uniform, approximately 50% proportional increase in the observed number of new disease occurrences, compared to predictions for healthy individuals. The results confirm anectdotal evidence that interactions between co-existing diseases and treatments can substantially inflate overall morbidity burden.  
- His project employed several analytical approaches including multistage models to characterise how disease incidence patterns with age, clustering diseases based on associations with major risk factors, and quantifying modifiable disease risks from modifiable exposures like smoking and obesity.
- Some diseases like COPD had over 90% of risk attributable to smoking, suggesting they would be dramatically reduced if smoking were eliminated. Anthony stresses in the final sentence of the paper's conclusions however [2], that the results should be treated with caution and repeated more carefully before forming conclusions about any specific disease. 
- Late-onset diseases like cancers or cataracts, exhibited very low risk early in life but rapidly escalating risk in older ages. Other more "sporadic" diseases have a low risk throughout life that increases only slowly with age, and from a statistical perspective, the results suggested that a substantial proportion of these might be avoidable with a healthy lifestyle. 

### Questions and Answers:

1) Why did he not build separate sex-specific models instead of adjusting a single model?
> He analysed men and women separately but adjusted for sex-specific factors in the model like hormone replacement therapy and parity for women. He could then remove these adjustment variables using marginalisation prior to clustering diseases.
2) Could the models assess how much excess morbidity burden could be avoided by reducing adverse medication effects in multimorbid patients?  
> No, he did not look at medications or their effects at all in this analysis. His aim was to quantify the increase in morbidity above that expected in otherwise healty individuals, that was potentially attributable to disease-disease and disease-treatment interactions.
3) For assessing multimorbidity, did he look at first ever occurrence of each disease or include subsequent occurrences as well?
> To maximise the number of diseases studied, he compromised by looking at the first occurrence of any disease within each ICD-10 disease chapter, though ideally first occurrence of any disease would have been preferable to avoid any interaction effects.  
4) Did he consider using competing risk models with a frailty term which could account for individuals with higher risk of multiple diseases?
> As detailed in the supplementary material of Ref. [3], he concluded that competing risk models were not required for estimating the underlying disease risks, though they would be needed to reproduce the exact observed morbidity patterns in the data (that depend on all diseases that might occur). 



