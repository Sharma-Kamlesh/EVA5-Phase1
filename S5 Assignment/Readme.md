###S5 Coding Drill Down


Step 1: [Code 1](https://github.com/Sharma-Kamlesh/EVA5-Phase1/blob/main/S5%20Assignment/S5_Code_1.ipynb)
  1.  Target:
        - Make the model lighter
  2.  Results:
        - Parameters: 7,730
        - Best Train Accuracy: 99.18
        - Best Test Accuracy: 98.97
  3.  Analysis:
        - Good model!
        - No over-fitting, model is capable if pushed further
 
 
Step 2: [Code 2](https://github.com/Sharma-Kamlesh/EVA5-Phase1/blob/main/S5%20Assignment/S5_Code_2.ipynb)
  1.  Target:
        - To increase the model efficiency, added batch normalization after each layer.
  2.  Results:
        - Parameters: 7,862
        - Best Train Accuracy: 99.63
        - Best Test Accuracy: 99.25
  3.  Analysis:
        - The Train Accuracy has increased consistently.
        - But we start getting overfitting after Epoch 6 

Step 3: [Code 3](https://github.com/Sharma-Kamlesh/EVA5-Phase1/blob/main/S5%20Assignment/S5_Code_3.ipynb)
  1.  Target:
        - add dropout with Normalization to avoid the overfitting and Add rotation transform
  2.  Results:
        - Parameters: 6,770 ( changed the model output and input channels)
        - Best Train Accuracy: 99.24
        - Best Test Accuracy: 99.35
  3.  Analysis:
        - Droput was making the model inconsistent and reducing the accuracy 
        - With removal of dropout the model increase the accuracy of the model and achieved 99.35 on 15th Epoch. 
