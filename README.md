# Bias-In-Pretrained-Models-Final-Project

**Reference / Citation  :** 
This codebase takes inspiration from the below reasearch paper to verify and replicate the results to quantify stereotypical bias in pretrained language models:  
  
@misc{nadeem2020stereoset,  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title={**StereoSet: Measuring stereotypical bias in pretrained language models**},  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;author={Moin Nadeem and Anna Bethke and Siva Reddy},  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;year={2020},  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;eprint={2004.09456},  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;archivePrefix={arXiv},  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;primaryClass={cs.CL}
}  
  
 ** Steps  to replicate :**  
 1) Clone the repository
 2) Install pacakges listed in requirements.txt
 3) Download pretarined model files from download_models.sh file from code/models/ folder
 4) Run the makefile to evalate biases for each model
 5) Run python3 evaluation.py --gold-file ../data/dev.json --predictions-dir predictions/ to score and generate the lms, ss and icat scores for each model.
 
** Note: Modifications to original setup**  
1) Wrote and fixed code in a few python files to make the 
2) Please ignore eval_ensemble.py and eval_sentiment_models.py. They are kept so that makefile doesn't break from the original StereoSet files.
3) Genrated 
