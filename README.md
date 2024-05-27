# Epidemiological Deep Neural Networks:

This is the official project worth 1 credit presented in the course Mathematical Modeling, at BITS Goa lectured by Dr. Anushaya Mohapatra. A supplement for the advanced knowledge of Epidemiological Compartmental Modeling was acquired through the Lecture Series by Dr. Abhishek Pandey, Yale University as a part of The SPARC Project, conducted in person at BITS Goa.

## MOTIVATION
Epi-DNNs (Epidemiological Deep Neural Networks) is a novel idea proposed by (Xiao Ning, Linlin Jia, Yongyue Wei, Xi-An Li, Feng Chen) in the paper (Epi-DNNs: Epidemiological priors informed deep neural networks for modeling COVID-19 dynamics) published in 2023 in the prestigious journal of (Computers in Biology and Medicine). The research paper is made available in this repository or plz visit [here](https://www.sciencedirect.com/science/article/pii/S0010482523001580). 

(Citation to the paper is uploaded in this repo; [License](https://creativecommons.org/licenses/by/4.0/))

## INTRODUCTION 
The Compartmental Model used here is not the original SEIRD model but a variation of the same, created due to the Type of Dataset obtained. The flow model for this project is: 
![Variation of SEIRD Model](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/d21b39dd-0e23-4e6f-874e-ced52fc58e24).

In the dataset:
The Initial Susceptible Population is the Total Indian Population before the start of Covid - 19 pandemic. The conversion rate from "Susceptible" to "Exposed" is termed as "Alpha"(Transmission Rate).
The "Exposed" Compartment is constituted by the Confirmed Cases column in the dataset.
The "Currently Infected" Compartment is the number of Active Cases and the conversion rate from "Exposed" to "Infected" is termed as "Beta".
The "Recovered" and the "Death due to infection" Compartments are clearly marked in the dataset as well, with rates "Gamma" and "Mu".

## IMPROVISATION
The algorithm is implemented on a variation of SEIRD Model and models the effect of the **Covid-19 pandemic in India**. Here the Susceptible Population is considered to be the Total Indian Population at the time of Covid - 19, Birth Rate and Natural Death Rate is neglected (as it will make the model much more complex). E,I,R,D are Exposed , Infected , Recovered and Death due to infection respectively. The dataset used is Collected by Ministry of Health and Family Welfare and Organised by PRS legislative research(present in the Github Repository) or [here](https://prsindia.org/covid-19/overview) / Kaggle.
(All the images are results obtained from the given code and dataset, figures can be easily cross-checked).

## RESULTS
The individually predicted compartment graphs for Susceptible, Exposed, Infected, Recovered and Deceased are attached below:
**For Epochs = 10:**
![SEIRD Graphs@10](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/3c4b711d-7ece-432e-b6e6-83f9093f5a2a)
**For Epochs = 50:**
![SEIRD Graphs@50](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/2e9925bd-eeaa-4f61-b339-3ba7f70a17cc)
**For Epochs = 100:**
![SEIRD Graphs@100](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/8095ffba-8513-4625-a65d-6c1c806806ab)

The plots for variation of predicted Parameters obtained from the Neural Network are shown below:(Alpha, Beta, Gamma, Mu)
**For Epochs=10:**
![Para values@10](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/c6b782db-605e-46ab-9356-ab00e5e3c7b6)
**For Epochs=50:**
![Para values@50](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/3b88f6a9-822d-4881-b136-d1a8582ead02)
**For Epochs=100:**
![Para values@100](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/0208be27-63a8-4f09-a106-164dae093262)

When we plot all the graphs (@100 epochs) together we see that, which leads to a very shocking revelation at first as we see the number of people affected out of India's total population at that time, i.e. 1,38,31,00,000 individuals
![Pred_Seird](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/f62e6b41-c772-4305-a6ed-b665f2c43cfa)

The number of Corona Virus Cases(as of 2024) in India are : 4,50,35,393 individuals

By only plotting the EIRD Graph we are able to perform a much deeper analysis:
![Pred_EIRD](https://github.com/MehShlok/Implementation-of-Epi-DNNs/assets/119751755/64170d35-3457-45fd-8a96-c9a394164384)


## FURTHER IMPROVEMENTS
Further Improvements: The realisation that this concept can be applied to almost all Epidemiological Compartment Models to make them much more efficient and to model any virus,disease,pandemics,epidemics.
Moreover this can be used to forecast future infectious diseases and their growth, precautions to be taken, various interventions that can be applied, etc.

(Thank you! [Yash Bhisikar](https://yashrb24.github.io/) and [Hardaat Singh Baath](https://hardaat-singh-baath.vercel.app/) for a thorough review of the project)
~Shlok Mehendale
