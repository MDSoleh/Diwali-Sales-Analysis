![diwalisales](https://github.com/MDSoleh/Diwali-Sales-Analysis/assets/99492800/65457d79-25ae-4139-9f37-02da12aed3b3)
# Diwali-Sales-Analysis
In this EDA project I analyse and visualize the business required questions.

## Install Libraries:

 - !pip install numpy                          
 - !pip install pandas                        
 - !pip install seaborn


# Steps involved before EDA:
### 1.Collect data:Here from a csv file.
 
 ### 2.Reading csv file.
 dframe = pd.read_csv(r"C:\Users\soleh\Downloads\Python Projects\Python_Diwali_Sales_Analysis-main\Diwali Sales Data.csv",encoding = 'unicode_escape')
 
### 3.Data-cleaning.
 
### 4.Droppping null values/blank columnsor unrelated columns.
 -dframe.drop(['Status','unnamed1'],axis = 1 , inplace = True)  : drop the blank/unrelated columns.
 -pd.isnull(dframe).sum()  : Gives count of null values.
 -dframe.dropna(inplace = True)  : Drop null values.
 -dframe['Amount'] = dframe['Amount'].astype('int') : Changing datatype. 

 #Conclusion

### Married women age group 26-35 yrs from UP, Maharastra and Karnataka working in IT, 
### Healthcare and Aviation are more likely to buy products from Food, Clothing and Electronics category
 
