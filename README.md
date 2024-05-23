Abstract
Background: The implementation of evidence-based clinical decision support systems (CDSS) has shown significant potential to enhance the safety, quality, and efficiency of healthcare services, as well as patient outcomes. This research explored the development of a Clinical Decision Support System for prescribing Combined Oral Contraceptives (CDSS-COCs) to reduce the incidence of venous thromboembolism (VTE) among users. The system is based on guidelines from the World Health Organization (WHO), the UK Medical Eligibility Criteria for Contraceptive Use (UKMEC), and the Centers for Disease Control and Prevention (CDC). Additionally, the feasibility of integrating this system into the Health Information System (HIS) in Finland was evaluated.

Methodology: A narrative literature review was conducted using Google Scholar, PubMed, Mendeley, and databases from Tallinn University of Technology and Tampere University of Technology. Both quantitative and qualitative methods were employed, including in-depth semi-structured interviews with an application developer and expert clinician, and online and paper-based questionnaires among prospective users.

Results: The proposed CDSS-COCs was successfully developed, incorporating six key risk factors: age ≥35 years, body mass index (BMI) > 25 kg/m², smoking status, personal history of VTE, family history of VTE, and the genetic factor V Leiden mutation. By considering these factors before prescribing COCs, the system aims to reduce VTE incidences by suggesting alternative treatments when risks are identified. The reliability and usability of the system were assessed from technical, user, and partially clinical perspectives. However, the immediate implementation of the system is limited by the lack of structured data in Electronic Health Records (EHR) concerning smoking status and family history. Additionally, the genetic factor V Leiden mutation is not universally available due to the absence of a mandatory screening policy in Finland.

Conclusion: This proposal has been designed as a practical tool to provide clinical decision-makers with direct consultation based on electronic patient data retrieved from digital repositories. By interpreting clinical guidelines from WHO, UKMEC, and CDC into a digital tool, the proposed system assists medical providers in prescribing the safest hormonal treatments for their patients, thereby promoting a personalized medicine approach.

# CDSS-COCs-Algorithm
This system helps clinicians make accurate hormonal treatment decisions, reducing VTE risk. CDSS-COCs evaluate six VTE risk factors  for COCs users. It generates three prescribing alarm messages and uses a four-level decision process to recommend alternative treatments if needed. 
The CDSS-COCs prototype system assesses six key risk factors for Venous Thromboembolism (VTE) in patients considering combined oral contraceptives (COCs). These risk factors include Age ≥35, BMI >25, Family History, Smoking, Personal History of VTE, and the genetic factor V Leiden Mutation. Based on these factors, the system generates three distinct alarm messages to guide clinical decisions:

⚠️ Alarm message #1: It’s time to prescribe the COCs! 💊
⚠️ Alarm message #2: Hey doc, maybe prescribe COCs, but keep an eye on things, yeah? 👀
⚠️ Alarm message #3: Whoa there, let’s check the purpose of the treatment. This message includes eight reasons for the treatment. The user selects one, and the system suggests an appropriate alternative treatment.
Decision Process Structure
The decision-making process in CDSS-COCs is divided into four levels, with the system advancing to the next level if the patient’s case does not match the current criteria:

Level 1: The system checks the criteria in List 1. If a match is found, Alarm message #3 is triggered. The user then selects the treatment purpose from a list, prompting the system to suggest an alternative treatment.
Level 2: If the patient’s case does not match List 1, the system evaluates the criteria in List 2. If a match is found, Alarm message #1 is generated, concluding the process.
Level 3: If the patient’s case does not match List 2, the system examines the criteria in List 3. If a match is found, Alarm message #2 is generated, concluding the process.
Level 4: If the patient’s case does not match List 3, the system checks the criteria in List 4. If a match is found, Alarm message #3 is generated, and the user proceeds as described in Level 1.
Criteria and Alternative Treatments
Table 1: List of Criteria
Table 2: List of Alternative Treatments
Table 3: Flowchart of the Proposed System CDSS-COCs
Table 4: Screenshot of the Prototype System
Conclusion
CDSS-COCs is designed to provide clinicians with precise recommendations for hormonal treatment, considering six major risk factors: BMI, Age, Smoking, Personal History of VTE, Family History of VTE, and the genetic factor V Leiden Mutation. By identifying patients at a higher risk of VTE during COCs treatment, the system aims to reduce VTE incidences among COCs users. This structured approach ensures that each patient receives a personalized assessment, leading to safer and more effective treatment decisions.

References
[1] H. L. Thacker, “Hormone Therapy and the Risk of Venous Thromboembolism,”2014, 
2016.
[2] D. a Brown and C. M. Vartan, “Risk of venous thromboembolism with drospirenonecontaining oral contraceptives,” Am. J. Health. Syst. Pharm, 2011.
[3] J. Brynhildsen, “Combined hormonal contraceptives: prescribing patterns, compliance, 
and benefits versus risks.” Ther. Adv. drug Saf, 2014.
[4] A. Pearson, A. Moxey, J. Robertson, I. Hains, M. Williamson, J. Reeve, and D. 
Newby, “Do computerized clinical decision support systems for prescribing change 
practice? A systematic review of the literature (1990-2007).” BMC Health Serv, 2009.
[5] S. Christin-Maitre, “History of oral contraceptive drugs and their use worldwide,” Best 
Pract. Res. Clin. Endocrinol. Metab, 2013.
[6] M. Conrad Stöppler, “Article ‘Birth Control Pills (Oral Contraceptives).” 
www.medicinet.com.
[7] Dawn Stacey, PhD, LMHC, July 14, 2016, Types of Combination Birth Control Pills 
Differences Between Monophasic, Biphasic and Triphasic Pills 
https://www.verywell.com/types-of-combination-pills-906935
[8] Trussell J, Contraceptive failure in the United States, Contraception, 2011
[9] A. E. Schindler, “Non-contraceptive benefits of oral hormonal contraceptives,” Int. J. 
Endocrinol. Metab, 2013.
[10] M. Serrani and J. T. Jensen, “Noncontraceptive benefits of the estradiol valerate / 
dienogest combined oral contraceptive : a review of the literature,” Int. J. Womens. Health, 
2014.
[11] T. W. Wakefield, D. D. Myers, and P. K. Henke, “Mechanisms of venous thrombosis 
and resolution,” Arterioscler. Thromb. Vasc. Biol, 2008.
[12] “American Heart Association, Venous-Thromboembolism-VTE_UCM_479052_Article 
@ www.heart.org, March (2017).”
http://www.heart.org/HEARTORG/Conditions/VascularHealth/VenousThromboembolism/
Venous-Thromboembolism-VTE_UCM_479052_Article.jsp
[13] J. A. Heit, F. A. Spencer, and R. H. White, “The epidemiology of venous 
thromboembolism,” J. Thromb. Thrombolysis, 2016.
[14] F. Editor-in-Chief Anthony J. Busti, MD, PharmD, FNLA and C. Reviewers: Jon D. 
Herrington, PharmD, BCPS, BCOP and Donald S. Nuzum, PharmD, BCACP, “oralcontraceptive-clotting-factors-thrombosis-dvt-pe @ www.ebmconsult.com:” 
[15] E. S. Berner, “Clinical decision support systems: state of the art,” Agency Healthc. Res. 
Qual, 2009.
[16] S. L. Tiffen J1, Corbridge SJ2, “Enhancing clinical decision making: development of a 
contiguous definition and conceptual framework.” NCPI US National Library of Medicine 
National Institutes of Health Search database Search term, 2014.
[17] I. Sim, P. Gorman, R. Greenes, and R. Haynes, “Clinical decision support systems for 
the practice of evidence-based medicine,”2001.
73
[18] D. F. Sittig, A. Wright, J. A. Osheroff, B. Middleton, J. M. Teich, J. S. Ash, E. 
Campbell, and D. W. Bates, “Grand challenges in clinical decision support,” J. Biomed. 
Inform, 2008.
[19] Commission European, “Country Brief : Finland,” 2010.
[20] Cohen D, Crabtree B. "Qualitative Research Guidelines Project." 2006. 
http://www.qualres.org/HomeUnst-3630.html
[21] A. Steckler, K. R. McLeroy, R. M. Goodman, S. T. Bird, and L. McCormick, “Toward 
integrating qualitative and quantitative methods: an introduction,” Health Educ. Q, 1992.
[22] EbMeDs, “scripts @ www.ebmeds.org/Reducing the risk of thrombosis in patients on 
hormone replacement therapy.” EbMeDs, 2016.
[23] Mehilainen Oy, “ en @ www.mehilainen.fi.” https://www.mehilainen.fi/en
[24] Norwegian Institute of Public Health, G. Framework, “GUIDES,” Nor. Inst. Public 
Health
[25] J. L. Kujovich, “Factor V Leiden Thrombophilia.” Genet. Med., 2011.
[26] K. W. Bloemenkamp, F. R. Rosendaal, F. M. Helmerhorst, H. R. Büller, and J. P. 
Vandenbroucke, “Enhancement by factor V Leiden mutation of risk of deep-vein 
thrombosis associated with oral contraceptives containing a third-generation progestagen,” 
Lancet, 1995.
[27] L. Kovacs, “Oral contraception over the age of 40,” Ann N Y Acad Sci, 2003.
[28] M. A. Stenchever, “Risks of oral contraceptive use in women over 35.” J. Reprod. 
Med., 1993.
[29] A. L. Nightingale, R. A. Lawrenson, E. L. Simpson, T. J. Williams, K. D. MacRae, and 
R. D. Farmer, “The effects of age, body mass index, smoking and general health on the risk 
of venous thromboembolism in users of combined oral contraceptives.,” Eur. J. Contracept. 
Reprod. Health Care, 2000.
[30] Centers of disease control, “Body mass index: Considerations for practitioners,” 2011.
[31] K. A. L. Darvall, R. C. Sam, S. H. Silverman, A. W. Bradbury, and D. J. Adam, 
“Obesity and Thrombosis,” Eur. J. Vasc. Endovasc. Surg., 2007.
[32] E. R. Pomp, S. Le Cessie, F. R. Rosendaal, and C. J. M. Doggen, “Risk of venous 
thrombosis: Obesity and its joint effect with oral contraceptive use and prothrombotic 
mutations,” Br. J. Haematol., 2007.
[33] J. T. Powell, “Vascular damage from smoking: disease mechanisms at the arterial wall.” 
Vasc. Med, 1998.
[34] V. Tzankova, V. Petrov, and N. Danchev, “Impact of Oral Contraceptives and Smoking 
on Arterial and Deep Venous Thrombosis: A Retrospective Case-Control Study,” 
Biotechnol. Biotechnol. Equip, 2014. 
[35] G. Hron, S. Eichinger, A. Weltermann, E. Minar, C. Bialonczyk, M. Hirschl, M. Stain, 
V. Gartner, and P. A. Kyrle, “Family history for venous thromboembolism and the risk for 
recurrence.,” Am. J. Med., 2006.
[36] A. L. Horton, V. Momirova, D. Dizon-Townson, K. Wenstrom, G. Wendel, P. Samuels, 
B. Sibai, C. Y. Spong, M. Cotroneo, Y. Sorokin, M. Miodovnik, M. J. O’Sullivan, D. 
Conway, and R. J. Wapner, “Family history of venous thromboembolism and identifying 
factor V Leiden carriers during pregnancy.,” Obstet. Gynecol., 2010.
74
[37] C. C. Trenor, R. J. Chung, A. D. Michelson, E. J. Neufeld, C. M. Gordon, M. R. Laufer, 
and S. J. Emans, “Hormonal Contraception and Thrombotic Risk: A Multidisciplinary 
Approach,” Pediatrics, 2011.
[38] Y. Vinogradova, C. Coupland, and J. Hippisley-Cox, “Exposure to combined oral 
contraceptives and risk of venous thromboembolism: a protocol for nested case-control 
studies using the Q Research and the CPRD databases.” BMJ Open, 2014.
[39] R. E. J. Roach, W. M. Lijfering, A. V. H. Vlieg, F. M. Helmerhorst, F. R. Rosendaal, 
and S. C. Cannegieter, “The risk of venous thrombosis in individuals with a history of 
superficial vein thrombosis and acquired venous thrombotic risk factors,” 2015.
[40] Healthit.gov, “Measure Effects and Refine CDS Interventions,” 2011.
