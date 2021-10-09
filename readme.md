# **[1st Place] Final IFest 2021 - Analisis Sentimen Kebijkakan PPKM Pemerintah**

At this final competition, we are given time for 5 hours with a task to make the best model for sentiment analysis from the given train and test data (non-label) about the Indonesia government rule, PPKM.

Authors (Yaudalah Team) :
1. [Ananda Affan Fattahila](https://github.com/Fanzru)
2. [Fendi Irfan Amorokhman](https://github.com/fendiirfan/)
3. [Kaenova Mahendra Auditama](https://github.com/kaenova)
4. [Kurniadi Ahmad Wijaya](https://github.com/ShinyQ)


## **Data Modelling Steps**
<img src="https://i.ibb.co/r2b29c0/Alur-Pemrosesan-drawio.png" alt="drawing" width="400"/>

Actually, At this phase, we tried several data cleansing techniques to find the best model accuracy. The list of it is :
- Stemming + Delete PPKM Words + Stopwords
- Stemming + Minimum 2 Words + Stopwords
- Stemming + Stopwords
- Non-Stopwords + Stemming + Minimum 2 Words 
- Non-Stopwords + Minimum 2 Words 
- Delete PPKM Words + Minimum 2 Words + Stopwords
- Non Stemming + Stopwords

We also do benchmark the model into the balance and unbalance data in . So, all of it was consist **16 Combination For each Models** 😱

![Multitask Spongebob](https://c.tenor.com/sqxKQ3lUS_wAAAAC/spongebob-spongebob-squarepants.gif)

We actually tuning the models for about 4 hours lol.

## **Benchmark Model Accuracy Results**

After benchamrking, we find out that Unbalance, Non-Stopwords, Stemming, and Minimum 2 Words cleansing give us the best accuracy. Below is the list of the best accuracy we got in some models.

| Model        | Validation Accuracy    |
| -----------  | ---------------------- |
| IndoBERTweet |     0.84               |
| IndoBERT     |     0.83               |
| LSTM         |     0.75               |
| biLSTM       |     0.75               |
| SVM          |     0.74               |
| Naive Bayes  |     0.62               |

As seen above the IndoBERTweet models give the highest accuracy so because no time left for another benchmark 😋 , it's time for us to predict the data test. 

In the end, the judge tells that we got the highest accuracy from other teams in the data test which has the accuracy of 0.79 and got the [1st Place](https://www.instagram.com/p/CUzfu7-Fk6y/), Horaay!!!
