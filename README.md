# SBSPS-Challenge-9303-Develop-and-Deploy-an-Application-for-Nutrition-Assistant
Develop and Deploy an Application for Nutrition Assistant

## Nutrition assistant

### IBM products used
1. IBM_db2
2. IBM watson studio
### Introduction

This is a web application which helps people to keep track of their health by finding and reporting the calorie intake and additionally it finds the BMI of the user with the help of their Height and Weight and it also provides a detail report for the user in the report tab.

## Application Structure

### LOG IN PAGE:
This page is used to grant acces to registered uses.To check whether the user has registered before or not we use  **IBM_DB2**.
when the user log's in using his/her crendentials it is automatically compared with all the entries in **IBM_DB2** and if a prefect match is found the user is redirected to **HOME PAGE**. 
If not the user is **not an authenticated user** then he is redirected to **register page.**

### Register page

This is the page where the new user can register. 
Users are requested to fill all the required details such as 
1.Name
2.E-mail
3.Password
4.Phone
The details filled by the user are then poured into **IBM_DB2.**
This data is later used by the webpage to validate the user in his future visits.
If the registration is successful then the user is redirected to LOGIN page where he/she should give her crenditials to login to HOME page.

### Home page

This is the page where the user can choose various options available such as

**1.BMI calculator
2.Calorie Count
3.Report**

### BMI calculator

This page uses **BMI model** which was trained to predict BMI value of a user with his Height and Weight.

#### Snapshot of Dataset use


### Calories

This page requests user to insert image of the food .This image is further send to food_Detection model to detect the food.This page also requests the user to enter the quantify of food intake in servings then the output from the model and this servings are both used to calculate the calorie of the food eaten by the user.

below is the snapshot taken during training of the model.

![image](https://user-images.githubusercontent.com/104611878/192081493-1308b6e9-b28d-4159-9f20-cc7c6d2cb8c7.png)
