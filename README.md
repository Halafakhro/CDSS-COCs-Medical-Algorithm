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
