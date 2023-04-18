# Personalized-Cancer-Diagnosis-using-Machine-Learning

![image](https://user-images.githubusercontent.com/115543070/232690704-6eb46240-0e1b-4964-9294-ca9213830781.png)



<h2> Description </h2>

A lot has been said during the past several years about how precision medicine and, more concretely, how genetic testing is going to disrupt the way diseases like cancer are treated.

But this is only partially happening due to the huge amount of manual work still required. Memorial Sloan Kettering Cancer Center (MSKCC) launched this competition, accepted by the NIPS 2017 Competition Track,  because we need your help to take personalized medicine to its full potential.

Once sequenced, a cancer tumor can have thousands of genetic mutations. But the challenge is distinguishing the mutations that contribute to tumor growth (drivers) from the neutral mutations (passengers). 

Currently this interpretation of genetic mutations is being done manually. This is a very time-consuming task where a clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based clinical literature.

For this competition MSKCC is making available an expert-annotated knowledge base where world-class researchers and oncologists have manually annotated thousands of mutations.
<h2> Dataset Description</h2>
- Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/data
- We have two data files: one conatins the information about the genetic mutations and the other contains the clinical evidence (text) that  human experts/pathologists use to classify the genetic mutations. 
- Both these data files are have a common column called ID
- <p> 
    Data file's information:
    <ul> 
        <li>
        training_variants (ID , Gene, Variations, Class)
        </li>
        <li>
        training_text (ID, Text)
        </li>
    </ul>
</p>

<h2>Problem Statement</h2>

 Classify the given genetic variations/mutations based on evidence from text-based clinical literature.
  

<h2> Business Constraints </h2>

1.Interpretability of the algorithm is must because a cancer specialist should understand why the model is given particular class so that he can explain to the patient.

2.No low-latency requirement which means patient can wait for the results. As there is no low-latency requirement, we can apply complex machine learning models.

3.Errors are very costly.

4.Probability of belonging to class is needed rather than it belonging to particular class.

<h2>Perfomance Metric </h2>

* Multi class log-loss 

* Confusion matrix 

<h2>Machine Learning Objective and Constraints</h2>
<p> Objective: Predict the probability of each data-point belonging to each of the nine classes.
</p>
<p> Constraints:
</p>

* Interpretability

* Class probabilities are needed.

* Penalize the errors in class probabilites => Metric is Log-loss.

* No Latency constraints.
