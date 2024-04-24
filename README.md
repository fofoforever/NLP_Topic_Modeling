# NLP_Topic_Modeling
by: Phuong Thao Nguyen 

Data was obtained from Kaggle but originally scraped from OkCupid, with usernames and dates removed for de-identification purposes. OkCupid users are categorized by sex and sexual orientation, with 20,533 straight females, 1,996 bisexual females, 1,588 gay females, 31,073 straight males, 3,985 gay males, and 771 bisexual males. Other information in the dataset includes typical user attributes such as age and ethnicity, as well as lifestyle variables like diet, drinking habits, and smoking habits. The dataset comprises ten essays per user, each capturing different facets of their personal lives, such as self-perception, activities, talents, social habits, cultural preferences, essentials in life, contemplative thoughts, typical Friday night activities, private admissions, and criteria for messaging potential matches. 

Dataset can be obtained here

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


CITATION: 

[1] Abram, M. D., Mancini, K. T., & Parker, R. D. (2021). Methods to integrate natural language processing into qualitative research. All Articles. https://doi.org/10.1177/1609406920984608

[2] Allen, J. P., Loeb, E. L., Kansky, J., & Davis, A. A. (2022). Beyond susceptibility: Openness to peer influence is predicted by adaptive social relationships. International Journal of Behavioral Development, 46(3), 180-189. https://doi.org/10.1177/0165025420922616

[3] Blot, W. J. (1992). Alcohol and cancer. Cancer Research, 52(7 Suppl), 2119s-2123s. PMID: 1544150.

[4] Dunbar, R. I. M., Launay, J., Wlodarski, R., et al. (2017). Functional benefits of (modest) alcohol consumption. Adaptive Human Behavior and Physiology, 3, 118–133. https://doi.org/10.1007/s40750-016-0058-4

[5] Duell, N., Clayton, M. G., Telzer, E. H., & Prinstein, M. J. (2022). Measuring peer influence susceptibility to alcohol use: Convergent and predictive validity of a new analogue assessment. International Journal of Behavioral Development, 46(3), 190-199. https://doi-org.proxy.library.vanderbilt.edu/10.1177/0165025420965729

[6] Flesia,Luca,Valentina Fietta, Carlo Foresta, and Merylin Monaro. 2021. The Association between Dating Apps and Alcohol Consumption in an Italian Sample of Active Users, Former Users, and Non-Users.SocialSciences10: 249. https://doi.org/10.3390/socsci10070249

[7]George, S., Rogers, R. D., & Duka, T. (2005). The acute effect of alcohol on decision making in social drinkers. Psychopharmacology, 182(1), 160-169. https://doi.org/10.1007/s00213-005-0057-9

[8] Huang, T.-F., Hou, C.-Y., Chang, F.-C., Chiu, C.-H., Chen, P.-H., Chiang, J.-T., Miao, N.-F., Chuang, H.-Y., Chang, Y.-J., Chang, H., & Chen, H.-C. (2023). Adolescent use of dating applications and the associations with online victimization and psychological distress. Behavioral Sciences, 13(11), 903. https://doi.org/10.3390/bs13110903

[9] Giorgi, S., Yaden, D. B., Eichstaedt, J. C., Ashford, R. D., Buffone, A. E. K., Schwartz, H. A., Ungar, L. H., & Curtis, B. (2020). Cultural differences in tweeting about drinking across the US. International Journal of Environmental Research and Public Health, 17(4), 1125. https://doi.org/10.3390/ijerph17041125

[10] Jelodar, H., Wang, Y., Rabbani, M. et al. A Collaborative Framework Based for Semantic Patients-Behavior Analysis and Highlight Topics Discovery of Alcoholic Beverages in Online Healthcare Forums. J Med Syst 44, 101 (2020). https://doi.org/10.1007/s10916-020-01547-0

[11] Jose, R., Matero, M., Sherman, G., Curtis, B., Giorgi, S., Schwartz, H. A., & Ungar, L. H. (2022). Using Facebook language to predict and describe excessive alcohol use. Alcoholism: Clinical and Experimental Research, 46(5), 836–847. https://doi.org/10.1111/acer.14807

[12] Marengo, D., Azucar, D., Giannotta, F., Basile, V., & Settanni, M. (2019). Exploring the association between problem drinking and language use on Facebook in young adults. Heliyon, 5(10), Article e02523. https://doi.org/10.1016/j.heliyon.2019.e02523

[13] OpenAI. (2024). ChatGPT (4) [Large language model]. https://chat.openai.com

[14] Peters, B. L., & Stringham, E. (2006). No booze? You may lose: Why drinkers earn more money than nondrinkers. Journal of Labor Research, 27, 411–421. https://doi.org/10.1007/s12122-006-1031-y

[15] Rudeboybert. (n.d.). OkCupid codebook (Revised). GitHub. https://github.com/rudeboybert/JSE_OkCupid/blob/master/okcupid_codebook_revised.txt

[16] Scannell, M. J. (2019). Online Dating and the Risk of Sexual Assault to College Students. Building Healthy Academic Communities Journal, 3(1), 34–43. https://doi.org/10.18061/bhac.v3i1.6688

[17] Stappenbeck, C. A., & Fromme, K. (2014). The effects of alcohol, emotion regulation, and emotional arousal on the dating aggression intentions of men and women. Psychology of Addictive Behaviors, 28(1), 10–19. https://doi.org/10.1037/a0032204

[18] World Health Organization. (n.d.). Alcohol. Retrieved from https://www.who.int/news-room/fact-sheets/detail/alcohol




