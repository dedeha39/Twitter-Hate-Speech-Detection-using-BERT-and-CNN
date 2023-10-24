# Twitter Hate Speech Detection

This repository contains the implementation for a hate speech detection system designed to safeguard young users on Twitter. The system employs advanced Natural Language Processing (NLP) techniques, integrating the BERT (Bidirectional Encoder Representations from Transformers) model and a Convolutional Neural Network (CNN) architecture. The research conducted in this project focuses on enhancing hate speech detection accuracy and improving the safety of social media platforms for children and adolescents.

## Table of Contents

- [Introduction](#introduction)
- [Approach](#approach)
- [Related Work](#related-work)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusions](#conclusions)
- [Future Work](#future-work)
- [References](#references)

## Introduction

Hate speech is a pervasive issue on social media platforms, especially affecting young users who are vulnerable to online harassment. This project addresses the problem of hate speech on Twitter by developing an automated detection system. The system leverages the power of BERT, a state-of-the-art NLP model, in conjunction with a CNN architecture to effectively identify hate speech instances in tweets.

## Approach

We utilized BERT (Bidirectional Encoder Representations from Transformers) models for hate speech detection. BERT's bidirectional nature allows it to understand the context of words in a sentence, making it effective for natural language processing tasks like hate speech detection.

## Related Work

Several studies have been conducted in the field of hate speech detection. Previous research includes methods using graph convolutional networks, machine learning algorithms like K-Nearest Neighbor and Naive Bayes, and linguistic analysis for different languages.

## Dataset

The dataset used in this research consists of tweets categorized into three distinct groups: hate speech, offensive language, and neither. The data was meticulously collected to facilitate hate-speech detection research and includes instances of racism, sexism, homophobia, and other offensive content. The dataset's diversity ensures a comprehensive analysis of hate speech patterns on social media.

## Methodology

Our approach employs a text-centric methodology, focusing primarily on tweets as the primary data source. The system utilizes BERT, a transformer-based neural network architecture, to learn contextual representations of words and sentences. Additionally, a CNN model is employed to capture local patterns and relationships within the text. The integration of BERT and CNN enables the system to analyze tweets comprehensively, enhancing the accuracy of hate speech detection.

## Results

We evaluated two BERT models for hate speech detection based on different configurations:

### Model 1: BERT L=12, H=768, A=12
- **Configuration:**
  - Number of Hidden Layers (L): 12
  - Hidden Size (H): 768
  - Attention Heads (A): 12

- **Performance Metrics:**
  - Accuracy: 91%
  - F1-Score: 0.78

### Model 2: BERT L=4, H=512, A=4
- **Configuration:**
  - Number of Hidden Layers (L): 4
  - Hidden Size (H): 512
  - Attention Heads (A): 4

- **Performance Metrics:**
  - Accuracy: 90%
  - F1-Score: 0.73

**Observations:**

The `BERT L=12, H=768, A=12` model outperformed the `BERT L=4, H=512, A=4` model in hate speech detection. The superior performance of the former can be attributed to its more advanced and deeper word embedding due to its neural network architecture. A higher number of hidden layers, larger hidden size, and more attention heads allow the model to capture more intricate features in the input data, resulting in better accuracy and F1-score.

However, it is worth noting that even with its high accuracy, the model occasionally confused hate speech with offensive speech. Further improvements are possible through additional data and continued training.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## References

-1. Richard Delgado and Jean Stefancic, “Understanding Words that Wound”, 2004, Westview Press

-2. Krause, N., Ballaschk, C., Schulze-Reichelt, F., Kansok-Dusche, J., Wachs, S., Schubarth, W., & Bilz, L. (2021). “Ich lass mich da nicht klein machen!“ – Eine qualitative Studie zur Bewältigung ¨ von Hate Speech durch Schüler/innen [I don’t let them get me down!”—A qualitative study on students’ coping with hate speech]”. Zeitschrift für Bildungsforschung, 11(1), 169–185.

-3. Simpson, Robert. (2019). ‘Won’t Somebody Please Think of the Children?’ Hate Speech, Harm, and Childhood. Law and Philosophy. 38. 10.1007/s10982-018-9339-3.

-4. Halevy, A.; Ferrer, C.C.; Ma, H.; Ozertem, U.;-Pantel, P.; Saeidi, M.; Silvestri, F.; Stoyanov, V. Preserving Integrity in Online Social Networks. arXiv 2020, arXiv:2009.10311

-5. Radfar, B.; Shivaram, K.; Culotta, A. Characterizing Variation in Toxic Language by Social Context. In Proceedings of the International AAAI Conference on Web and Social Media; Association for the Advancement of Artificial Intelligence: Menlo Park, CA, USA, 2020; Volume 14, pp. 959–963.

-6. Guberman, J.; Schmitz, C.; Hemphill, L.
Quantifying toxicity and verbal violence on Twitter.
In Proceedings of the 19th ACM Conference on
Computer Supported Cooperative Work and Social
Computing Companion, San Francisco, CA, USA,
27 February–2 March 2016; pp. 277–280.
7. Gunasekara, I.; Nejadgholi, I. A review of standard
text classification practices for multi-label toxicity
identification of online content. In Proceedings of
the 2nd Workshop on Abusive Language Online
(ALW2), Brussels, Belgium, 31 October–1
November 2018; pp. 21–25.
8. Parent, M.C.; Gobble, T.D.; Rochlen, A. Social
media behavior, toxic masculinity, and depression.
Psychol. Men Masculinities 2019, 20, 277.
9. Poletto, F.; Basile, V.; Sanguinetti, M.; Bosco, C.;
Patti, V. Resources and benchmark corpora for hate
speech detection: A systematic review. Lang.
Resour. Eval. 2020, 55, 477–523 .
10. Davidson, T.;Warmsley, D.; Macy, M.;Weber, I.
Automated Hate Speech Detection and the Problem
of Offensive Language. arXiv 2017,
arXiv:1703.04009.
11. Mishra, P.; Del Tredici, M.; Yannakoudakis, H.;
Shutova, E. Abusive Language Detection with
Graph Convolutional Networks. In Proceedings of
the 2019 Conference of the North American
Chapter of the Association for Computational
Linguistics: Human Language Technologies,
Volume 1 (Long and Short Papers), 2019;
Association for Computational Linguistics:
Minneapolis, MN, USA, 2019; pp. 2145–2150.
12. Waseem, Z.; Hovy, D. Hateful Symbols or Hateful
People? Predictive Features for Hate Speech
Detection on Twitter. In Proceedings of the NAACL
Student Research Workshop, San Diego, CA, USA,
13–15 June 2016; Association for Computational
Linguistics: San Diego, CA, USA, 2016; pp. 88–93.
13. Waseem, Z. Are You a Racist or Am I Seeing
Things? Annotator Influence on Hate Speech
Detection on Twitter. In Proceedings of the
FirstWorkshop on NLP and Computational Social
Science, Austin, TX, USA, 5 November 2016;
Association for Computational Linguistics: Austin,
TX, USA, 2016; pp. 138–142.
14. Jaki, S.; Smedt, T.D. Right-wing German Hate
Speech on Twitter: Analysis and Automatic
Detection. arXiv 2019, arXiv:1910.07518
15. A. Chiu, K. Sood, A. Rincon and D. Doran,
"Detecting Hate Speech on Social Media with
Respect to Adolescent Vulnerability," 2023 IEEE
13th Annual Computing and Communication
Workshop and Conference (CCWC), Las Vegas,
NV, USA, 2023, pp. 0724-0728, doi:
10.1109/CCWC57344.2023.10099373.
16. Poletto, F.; Stranisci, M.; Sanguinetti, M.; Patti, V.;
Bosco, C. Hate speech annotation: Analysis of an
italian twitter corpus. In Proceedings of the 4th
Italian Conference on Computational Linguistics,
CLiC-it 2017, CEUR-WS, Rome, Italy, 11–13
December 2017; Volume 2006, pp. 1–6.
17. Pereira-Kohatsu, J.C.; Quijano-Sánchez, L.;
Liberatore, F.; Camacho-Collados, M. Detecting
and monitoring hate speech in Twitter. Sensors
2019, 19, 4654.
18. Vaswani, A.; Shazeer, N.; Parmar, N.; Uszkoreit, J.;
Jones, L.; Gomez, A.N.; Kaiser, L.u.; Polosukhin, I.
Attention is All you Need. In Advances in Neural
Information Processing Systems; Guyon, I.,
Luxburg, U.V., Bengio, S., Wallach, H., Fergus, R.,
Vishwanathan, S.,Garnett, R., Eds.; Curran
Associates, Inc.: New York, NY, USA, 2017 ;
Volume 30.
19. Devlin, J., Chang, M.W., Lee, K, Toutanova, K.,
“BERT: Pre-training of Deep Bidirectional
Transformers for Language Understanding”, 2019,
Proceedings of NAACL-HLT 2019, MN, USA,
pp-4171-4186
20. Peters, M. E., Neumann, M., Iyyer, M., Gardner,
M., Clark, C., Lee, K., Zettlemoyer, L. “Deep
contextualized word representations”, 2018,
NAACL 2018, arXiv:1802.05365v2
21. Radford, A., Narasimhan, K., Salimans, T.,
Sutskever, I., “Improving Language Understanding
by Generative Pre-Training”
22. Ozler, K.B.; Kenski, K.; Rains, S.; Shmargad, Y.;
Coe, K.; Bethard, S. Fine-tuning for multi-domain
and multi-label uncivil language detection. In
Proceedings of the Fourth Workshop on Online
Abuse and Harms, 2020; Association for
Computational Linguistics: Stroudsburg, PA, USA,
2020; pp. 28–33.
23. Koufakou, A.; Pamungkas, E.W.; Basile, V.; Patti,
V. HurtBERT: Incorporating Lexical Features with
BERT for the Detection of Abusive Language. In
Proceedings of the Fourth Workshop on Online
Abuse and Harms, Online, 20 November 2020;
Association for Computational Linguistics:
Stroudsburg, PA, USA, 2020; pp. 34–43.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.


