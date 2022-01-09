# Data Biography

### Declaration of Authorship

I, [Haofu Wang], confirm that the work presented in this assessment is my own. Where information has been derived from other sources, I confirm that this has been indicated in the work.

[Haofu Wang]

Date of signature: 26 Nov 2021
Assessment due date: 26 Nov 2021
Student Number: 21112657

_Please write your answer immediately below the level-3 headers and delete the guidance prior to submission._

---

### 1. Who collected the data?

A: The data was collected from Inside Airbnb who focuses on analyzing the inner pattern of the publicly available data from a city’s Airbnb listings [1].

---

### 2. Why did they collect it?

A: The data was collected to support the data transparency and discover the impact of the short-term rentals of Airbnb on the city. Inside Airbnb thought that the results of the data were contrary to the Airbnb’s claimants [2]. Multiple questions including the details of the rentals can be generated with the data of the listings. 

---

### 3. How was it collected?

A: With the help of programming languages, the public dataset of the listings was collected from the website of Airbnb including the compiled names, locations, listings and other rental information [1]. Some of the data was calculated with the Occupancy Model such as the availability of a listing in the future which is one of the most important columns in the dataset [1]. Others was calculated by the aggregation of the listings such as the number of the listings the host currently has.

---

### 4. What useful information does it contain?

A: Although the actual address of the listing isn’t available on the Airbnb website, with the latitude and longitude we are still able to locate the listing to a rough area. Some other columns show the number of nights stay for the listing. The maximum night value and the availability in the future may reveal that Airbnb has dishonest circumstances that some listings were rented all over the year. An analysis can be made based on the number of the incidents and the location of the listings. An overall report can also be conducted based on the incidents. 

---

### 5. To what extent is the data 'complete'?

A: Inside Airbnb published this dataset of listings to discover the impact of the short-term rentals on London. However, all the listings in the form were scraped by Inside Airbnb in August 2020. As a result, it is impossible to make a comparison with the data in several different months and years. The data itself based on one-month doesn’t have the integrality for the examination. It also influences that the data cannot show the change of the listing from the host and Airbnb. Inside Airbnb claims that the data was scraped using the tool of some programming languages including Python. Due to the systematic problem, the data cannot differentiate the unavailable status and the booked status which may cause a series of analysis mistakes. When the scraper looped over the website, it might happen that some critical information was missing and misinput. For example, in the column of has_availability where the value should be Booleans, some of them are integers. The same situation also extends to last_scraped.

---

### 6. What kinds of analysis would this support?

A: Before we conduct any analysis, the first thing we should do is to deal with the NaNs and Nulls by identifying whether it is a systematic problem or an actual data. One of the analyses that can be conducted is a density map of the listings. For example, since the aim is to find out whether there are inappropriate long-term rentals of Airbnb, we need to set the target of the density map to the entire apartment/home rentals. The parameter shown in the map is maximum_nights_avg_ntm which is the average value of the maximum night booked in the next 365 nights [3]. The criteria boundaries can be set as 14 nights, 30 nights and 90 nights. With the detail of listings’ longitude and latitude set in WGS84 format, a density map can be drawn, by which we can learn the main distribution of the long-term-rentals’ location. The second analysis can be a histogram showing the percentage of the availability in the next 365 days of the listings. The criteria could be divided into larger than 335 days, larger than 305 days but smaller than 335 days, larger than 275 days but smaller than 305 days, and smaller than 275 days. The histogram can directly show the proportion of long-term rentals. 

---

### 7. Which of the uses presented in Q.6 are _ethical_?

A: When it comes to the ethical issues, privacy is an essential problem that must be discussed. According to the Disclaimers of Inside Airbnb, all the listing data in the form is objective and doesn’t involve the private information since the details of the host are presented in Airbnb. To be specific, Inside Airbnb claims that all the location data for the listings is collected from Airbnb that is anonymous and illegible, which means it cannot be located to a specific address but a rough area. Furthermore, Inside Airbnb removed some irrelevant information from the data form since the last version such as zipcode and street name which may cause the leak of private information. As a result, when we try to use the location data to conduct the density map, it is helpful for us to protect the location privacy for the host of the listings. What’s more, in the second analysis, the availability of nights is also calculated based on the calendar of Airbnb. There is no private information involved during the process. 

The ethical issues also extend to the discrimination against various aspects such as ages, sexuality and races. The information such as races and locations of host is sometimes used to compared with the race distribution of the listing area [4]. Inside Airbnb chooses to not include those kinds of private information to the dataset which could be easily obtained based on the host picture and description. 

Although Inside Airbnb values the importance of private information and tries various methods to protect the host’s privacy, it is inevitable that the ethical problem still exists. 
Nowadays, due to the method of big data, an intimate insight can be generated with the combination of multiple datasets [5]. Since the datasets in Inside Airbnb is open to public, there are thousands of data combinations of the listings. Although the single column of data may protect the privacy temporarily, the combinations of the analysis results could still cause a leak of private information. For example, the number of listings the host currently owned is presented in the dataset. By combining with the locations, more detailed ownership information can be deducted.


## Bibliography

[1] Murray Cox. (2021). About Inside Airbnb [Online]. Available: http://insideairbnb.com/about.html
[2] Murray Cox. (2021). Behind Inside Airbnb [Online]. Available: http://insideairbnb.com/index.html
[3] Murray Cox, “Inside Airbnb Data Dictionary”, Aug. 2020 [Revised Aug. 2002].
[4] D. Wachsmuth and A. Weisler, "Airbnb and the rent gap: Gentrification through the sharing economy," vol. 50, no. 6, pp. 1147-1170, 2018.
[5] K. Crawford and J. J. B. R. Schultz, "Big data and due process: Toward a framework to redress predictive privacy harms," vol. 55, p. 93, 2014.

## Appendix 

