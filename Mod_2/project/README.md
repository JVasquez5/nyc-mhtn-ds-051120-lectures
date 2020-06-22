# Module 2 Final Project

## Introduction

The goal of this project was to analyze data from a dataset and create a multivariate linear regression(MLR) model. I wanted to investigate the relationship between life expectancy against health behaviors. I decided to search the internet for said information luckily the following website had all the information I was looking for and more: County Health Rankings (https://www.countyhealthrankings.org). 

The aforementioned dataset was cluttered and filled with information that was not applicable or neccessary for the MLR. Therefore, I underwent a Data Cleaning process that involved the Pandas library. Furthermore, for both the analysis and visualizations I utilized Pandas, MatPlotLib, and Seaborn. Addtionally for hypothesis testing and modeling I used Scipy, Sklearn, and statsmodels. 

Once I complied and reviewed 3,193 counties/50 states worth of information I was able to uncover treads dicating what life expectancy should be on a county/state level. 

Thus, the crux of my missing was uncovering if there is a correlation between health behaviors, clinical care access, socioeconomic factors, and physical environment features and life expectancy.

## Business Case

As an insurance company looking to analyze premiums for the following year, can Health Behaviors, Clinical Care Access, Socioeconomic Factors, and Physical Enviornment predict Life Expectancy.

## High-Level Overview of Data

The dataset contained the following features:

(Target)
* life_expectancy

(Classification)
* fips_code                                                 
* state                                                     
* name   

(Health Behaviors)
* poor_or_fair_health                                       
* monthly_poor_physical_health_days                         
* monthly_poor_mental_health_days                           
* adult_smoking                                             
* adult_obesity                                             
* physical_inactivity                                       
* access_to_exercise                                        
* excessive_drinking                                        
* diabetes_prevalence                                       
* hiv_prevalence  
 
(Clinical Care Access)
* primary_care_physicians                                   
* dentists                                                  
* mental_health_providers 
* other_primary_care_providers
* flu_vaccinations  
* uninsured_under_65 
* uninsured_adults                                          
* uninsured_children  

(Socioeconomic Factors)
* median_household_income 
* high_school_grad                                          
* some_college                                              
* unemployed                                                
* children_in_poverty                                       
* single_parent_households 
* limited_access_to_healthy_foods
* children_eligible_for_free_or_reduced_price_lunch
* social_associations 
* homeownership                                             
* severe_housing_cost_burden
* proficient_in_English

(Physical Environment)
* severe_housing_problems                                   
* households_with_high_housing_costs                        
* households_with_overcrowding                              
* households_with_lack_of_kitchen_or_plumbing_facilities                                
* alcohol_impaired_driving_deaths                           
* drug_overdose_deaths                                      
* motor_vehicle_crash_deaths          
* homicides                                                 
* firearm_fatalities                                        
* violent_crime                                             
* injury_deaths                            
* population                                                


## Methodology

* Data Collection

* Data Wrangling

* EDA and Visualization

* Hypothesis Testing

* Model Development

* Cross Validation

## Results

* #1 Original Training Error:  1.5740083080327474 #1 Original Testing Error:  1.636546615939479
* #2 Poly Training Error:  1.0298128498262626 #2 Poly Testing Error:  2.0133305119976903
* #3 F-Test Training Error:  1.68099129161024 #3 F-Test Testing Error:  1.7207811862491273
* #4 Recursive Training Error:  1.6556114118543859 #4 Recursive Testing Error:  1.9505313413421144
* #5 Lasso Training Error:  1.013250246782096 #5 Lasso Testing Error:  1.6516859432780284

* Lasso Model Root Mean Squared Error Z-score: 0.5586994655577765

## Conclusion 

* Lasso test most successful
* RMSE error Z Score of 0.5586994655577765
* Able to predict life expectancy within 1 standard deviation of population mean

# Future work

* Pinpoint specific counties, within states with lowest life expectancy, and create model and compare to original.
The counties in Mississippi, state with lowest life expectancy, F-Test model had RMSE Z-score of ~0.6136, similar to   overall model. 
* Separate out the categories (Health Behaviors, Clinical Care Access, Socioeconomic Factors, Physical Environment) to establish true weight on life expectancy.
* From influx of money from "defund the police" work with state legislators to allocate resources accordingly for health/social reforms.
    