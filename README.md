# kaggle-atom-notebook
So basically we want to predict magnetic interaction between the atoms of the molecules called scalar coupling
STEPS:
1) First we learn about the target variable , what is scalar coupling , and its means , standard deviation, and its destribution with histogram 
2) then there are 8 types of coupling , we have to find the correlation between target and them.
3)then we merge the structural data with our main data with molecular name and atom_index.
4)the average distance between coupling atoms is likely to increase as a result of a longer coupling pathway, ergo more intervening bonds(1J, 2J, 3J), so distance can be a good feature
5)i have done label encoding for the type, atom_0 and atom_1 , because it can help to improve accuracy
6)i have tried lgb model , because it the fastest , and i think it is hit and trial method , i would do xgboost after that if i had time 
7)for performance metric mean absolute error works best as scalar coupling is continous and MAE works well , we can use mean square error as well
