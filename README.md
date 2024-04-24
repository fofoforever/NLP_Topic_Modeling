# NLP_Topic_Modeling

Data was obtained from Kaggle but originally scraped from OkCupid, with usernames and dates removed for de-identification purposes. OkCupid users are categorized by sex and sexual orientation, with 20,533 straight females, 1,996 bisexual females, 1,588 gay females, 31,073 straight males, 3,985 gay males, and 771 bisexual males. Other information in the dataset includes typical user attributes such as age and ethnicity, as well as lifestyle variables like diet, drinking habits, and smoking habits. The dataset comprises ten essays per user, each capturing different facets of their personal lives, such as self-perception, activities, talents, social habits, cultural preferences, essentials in life, contemplative thoughts, typical Friday night activities, private admissions, and criteria for messaging potential matches. 


Source: https://github.com/rudeboybert/JSE_OkCupid/blob/master/okcupid_codebook_revised.txt
https://www.kaggle.com/datasets/bryanteh/profiles-dating-app

#Research Goal

In this research, we aim to harness natural language processing (NLP) and machine learning techniques to explore the influence of alcohol consumption on user self-descriptions within the dating app OkCupid. As a platform that pairs users based on their self-descriptions and responses to specifically crafted essay prompts, OKCupid also compiles additional data, such as age and recreational drug use, which could further impact user interactions and preferences. Through a detailed analysis of these self-descriptions, our study seeks to uncover how alcohol consumption is reflected in the way users present themselves and search for matches. We anticipate identifying patterns that not only correlate with alcohol use but also interlink with other behaviors and preferences articulated in their profiles. By leveraging NLP, we will process and analyze the textual data from user profiles, aiming to deepen our understanding of the group dynamics related to alcohol consumption in the context of online dating.

**Primary Research Question:** Can we differentiate between frequent vs. non-frequent drinkers based on their OkCupid profiles? What terms differentiate these groups?

**Secondary Research:** How do topics, extracted from OkCupid profiles using [topic-modeling method], vary across the frequent and non-frequent drinker groups?

**Primary Hypothesis:** Based on the self-descriptions of users on OKCupid, it is possible to differentiate between them. Users who frequently drink are likely to have descriptions that reflect social outings and activities, just as those who drink less or not at all will exhibit similar traits in their profiles. Whereas infrequent drinkers or non-drinkers might emphasize interests in lifestyle or hobbies. It is expected that the content of these descriptions will gravitate towards themes reflective of their respective drinking habits.

**Secondary Hypothesis:** In addition, it is hypothesized that frequent drinkers will express topics related more to social events, such as large gatherings, to express their extroverted personality. While infrequent drinkers will express topics in regards to more one-on-one interactions or their interpersonal relationships. 


Steps Involve: 

1. In our investigation, we will break our analysis into two steps. First using logistic regression with TF-IDF as the features to see if we can differentiate between frequent users and infrequent alcohol users by just text descriptions of the users. If this method is successful, we understand that text-based can be used to differentiate the two and then proceed to look at topics within each essay or prompt.
2. Used Elbow Test and Sihlouette Score to find ideal number of topics
3. NMF to retrive top words for each topics
4. 


