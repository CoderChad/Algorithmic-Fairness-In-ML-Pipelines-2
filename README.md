# Algorithmic-Fairness-In-ML-Pipelines-2
This report outlines fairness enhancing interventions that I implemented into a Machine Learning Pipeline. I was interested in using the Machine Learning Algorithm to predict an individuals likelihood of being high or low income using sex as the sensitive attribute of analysis. 


# Please see the attached notebook for my work.



## Performance Analysis Metrics:

(i) Overall accuracy


(ii) Accuracy for the privileged group


(iii) Accuracy for the unprivileged group


(iv) Disparate Impact


(v) False positive rate difference

# Baseline Performance; 
<img width="543" alt="Screen Shot 2022-04-19 at 2 12 50 PM" src="https://user-images.githubusercontent.com/97006483/164068855-bd94b704-65de-4240-9047-e08ad0a08c9c.png">

# Methodology (Doings):

  1. Train a baseline random forest model to predict income
  2. Use Disparate Impact Remover (DI-Remover -- a pre-processing fairness-enhancing intervention by Feldman et al., 2015 ((https://arxiv.org/pdf/1412.3756.pdf)) that is implemented in AIF360)
  3. Measuring the affect on fairness and accuracy by adjusting  the repair level at five different values.
  4. Training a random forest model on each of the 5 transformed datasets
  5. Observing and noting the differences between the baseline random forest model and the new models using the same 5 aformentioned hyperameters.
  6. Note changes corresponding to varrying levels of repair. 


# Conclusion (Findings):

<img width="1440" alt="Screen Shot 2022-04-19 at 2 14 10 PM" src="https://user-images.githubusercontent.com/97006483/164069044-f238462f-1854-4d00-9241-4da6e8d0789a.png">

