
# Texas Datahack 2018

## Education in India

When India got independence from British in 1947 the literacy rate was 12.2% and as per the recent census 2011 it is 74.0%. Although it looks an accomplishment, still many people are there without access to education.

Here, we take a look [at a recent dataset](https://www.kaggle.com/rajanand/education-in-india) and try to find some insight.

Is there a correlation between students with disabilities and how often they are held back to repeat a grade? How do classroom conditions affect the rate at which students repeat a grade? Does literacy rate compared with repeat rate in a region give an accurate representation of the overall intelligence of students?

### Our Hypothesis
* Students with disabilities may need more attention in the classroom and we believe this may be contribute to a disproportionate amount of students repeating grades.

* Good classroom conditions, in fact, will increase students incentive to come to school and foster a better environment for learning, thus decreasing the rate at which students repeat grades.

* Tracking intelligence as a metric can accurately be measured by the literacy rate and amount of students who repeat a grade in each region; a higher literacy rate in that region should imply more parents are able to provide academic support outside of the school system and increase students success

### Our Process
We focused on the following: Repetition rates of students in class; impact of the number of students with disabilities with respect to repetition rates; impact of class conditions on repetition rate and impact of literacy of the district on the student repetition rate.
Results
We assigned a rank to the Districts based on how well they were performing and saw the best result in Aizawl, Mizoram: Literacy Rate: 98.5%; Repetition Rate: 3.3E-5. Hence only 0.003% of overall students repeat classes.
We utilized the following criteria to rank a state:
rating = (literacy_rate - (WEIGHT * repetition_percentage_in_district))/100
Interestingly, we saw only a small value of correlation 0.01 between students with disabilities and repetition rates. Hence its not necessary that students with disability have a higher rate of repetition.
We also used linear regression to find a pattern in repetition rate against classrooms with good conditions, bad conditions, and worse conditions.
The regression resulted in R^2 = 0.04347751800193013, R^2 = 0.06733208652703454, and R^2 = 0.015255590064973193, respectively. Although the model isn’t reliably strong (as the R^2 values are not quite high), the general pattern of the model shows that repetition rates are, in fact, negatively correlated with good classroom conditions, and positively with bad and worse conditions. Other detailed statistics of the data can be found in our GitHub repository, listed below.

###Conclusion
We found several interesting results in our search. Firstly, we found that disabilities do not greatly impact a student’s potential to pass and do well.
We found that classroom condition does impact the repetition rates of students
Thirdly, we also saw that states with high literacy rates usually had low repetition rates, hence having support from family and awareness of education impacts the performance of students.

[More Here](https://docs.google.com/document/d/1uUkKJZGiBTBfU0Gq2RRU60IHA0QyWTX6UDMianzSZdo/edit?usp=sharing)
