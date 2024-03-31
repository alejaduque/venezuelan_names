# Character-based language models of spanish dialects (Spanish and Venezuelan)

Character-based language models for generating names based in a Peninsular Spanish and Venezuelan corpus. 

# What will I find in this repository?

In this repository you will find two different applications of a character-based language model based on Andrew Karpathy's "make more" model (https://github.com/karpathy/nn-zero-to-hero/blob/master/lectures/makemore/makemore_part2_mlp.ipynb), which here is applied for two different datasets of spanish dialects, peninsular spanish and venezuelan spanish. 

This adaptation was done for a two part task. For the first part, we focused on adapting Kaparthy's model for the two datasets and evaluated its perfomance quantitatively and qualitatively. For the second part we focused on improving the dataset with the poorest performance, the venezuelan spanish, and adapted the model for it to return better metrics. For this purpose, we changed the hyperparamenters of the venezuelan dataset, extended the training corpus and the human evaluation for this dataset, collecting data from the evaluation of 81 anonymous users who qualitatively assesed a sample of our model's output. 

Thus, in this dataset you will find an improve version of the venezuelan dataset model, our original version for the peninsular spanish dataset, all the data necessary for training the models and later analysis of the data. 

# How to run

To install dependencies run the following code on terminal:
```
cd "PATH_TO_FOLDER_ORIGIN"

pip install -r requirements.txt

```
The ZIP folders contain: 
* corpus --> corpus used to train the models. Including the EXTENDED corpus of venezuelan model.
* name_collection --> venezuelan names collected in the survey
* human_evaluation --> lists of names generated by the language model and human-reviewed version of them. Including the data of EXTENDED evaluation.

The .ipynb files include
* organize_corpus.ipynb --> code for the organization of the data obtained from the survey (for the collection of Venezuelan names).
*  name_predictor_esp.ipynb --> code of character-based language model for Peninsular spanish.
*  name_predictor_vzl.ipynb --> ENHANCED code of character-based language model for Venezuelan spanish.
* evaluation_analysis.ipynb --> code for analysing the data from the human evaluation survey of VENEZUELAN dataset.




