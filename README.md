# R
Regression Analysis - Call Data
Set Working Directory = Downloads
Import Data to Excel
Save as CSV - Delimited

CallData = read.csv("DocName.csv")
summary(CallData)
str(CallData)
table(CallData$LDR.Call.Type, CallData$Title)
install.packages("mice")
library(mice)
Model1 = glm(LDR.Call.Type ~ ., data = CallData)
