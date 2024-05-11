# Applied Artificial Intelligence Coursework Repository

This repository contains my coursework for the Applied Artificial Intelligence course at my university (UNIFEI) which uses the PBL (Problem Based Learning) method as a teaching method. The coursework primarily consists of Jupyter notebooks containing solutions to the assignments.

## Assignments

### Assignment 1: Dysphagia Detection and Analysis

#### Introduction

Dysphagia is the difficulty in swallowing food or drinks. It can affect health and well-being, so it's important to detect its signs early. Elderly people and those with diseases such as Parkinson's disease, Alzheimer's disease, dementia, head and neck cancer, or a history of stroke may have difficulties swallowing.

#### New Non-Invasive Procedure

A growing array of technologies is currently available to assess various aspects of swallowing function and dysfunction. These technologies allow the measurement of the movements of the structures involved and muscle action through spatial and temporal aspects.

The equipment used for the swallowing study with the Doppler Sonar was the ULTRASONIC DETECTOR (portable), model DF-4001, from the MARTEC brand. The ultrasound frequency by the Doppler effect is 2.5 MHz, with an output of 10 mW/cm2. The sound output power is 1W.

![exam_image](https://lh7-us.googleusercontent.com/KX7F05Ki9kmIZn9EoWhOowEeu2EnJxfkSnfOSy0hq7KbYVkLSaW5hvFFMN6nOOw_vAZNN1Y0JEKxikAaZSaW75vy1PUZw4v7DblNl5OyWvEMh3kAEGP4qTjX-3JIKpzSdufeNwpnkOaEMD6LXd8LmSQ)

#### Dataset

The dataset was generated from 490 exams, which are sound signals from low-cost fetal ultrasonic dopplers, performing the procedure described in the introduction. Important points about the existing files:

- The Doppler has low noise filtering, so background noise is present in almost all measurements.
- The files have not been verified, so there are files that are not real clinical measurements.
- There are measurements without any swallowing or with many noises, being invalid for use.
- The number of swallows per measurement can vary from 1 to 4.

![comercial_ultrassom](https://lh7-us.googleusercontent.com/svnZGhpBlIjRRoKLrT9owh4rQNaqe-vS4rwTy7TAUxxdauHAoXqswPF9VHj_GT1qqNJ9bLox9k2fwxNT74rruZ1YxAnDvdKtKCAGXYzRTu6ixdm9SzqFcHzj9VXOpYlrBghUGvGCQQj7ZgGMAqE_RPw)

The dataset is available for download at the following address:
https://drive.google.com/file/d/1z1sqrxP_Ozdcu3sKvJDN7GJIxrv5TXBu/view?usp=drive_link

#### Steps

- Identify valid and invalid files in the dataset for training and testing from unsupervised learning.
- List best classic learning methodologies by cross-validation and hyperparameter search by balanced accuracy metrics to identify valid files from invalid ones.
- Use deep learning models to identify the periods of swallowing from the audio windows.


### Assignment 2: Folha de S.Paulo News Analysis

#### Introduction

![image.png](https://lh7-us.googleusercontent.com/TFpDkvdRc9fCvOKBI4uDCmApDRaCeLoFjq3doHqrzyX6iRhLKEoXLo-VBWU--ifkJ9lFD8T9lpm7h1dmZsnxihZsKpN80rA6Olu2q9DLxYgSFZehzNFeaPGeSuIUmUgOki7N4LBjkgHPz14itYG2GBQ)

Folha de S.Paulo, also known as Folha de São Paulo or simply Folha, is a Brazilian newspaper edited in the city of São Paulo. As of December 2021, it is the second largest newspaper in Brazil in circulation, with 366,087 copies (including digital subscribers), according to the Institute Verifier of Communication (IVC), trailing only behind the Rio de Janeiro newspaper, O Globo.

Founded by a group of journalists led by Olival Costa and Pedro Cunha on February 19, 1921, Folha was created in opposition to the main city newspaper, O Estado de S. Paulo, which represented the rural elites and assumed a more conservative, traditional, and rigid position.

#### Dataset

The dataset used in this assignment is sourced from Kaggle and consists of 167,053 news articles from the Folha de São Paulo website. Font: https://www.kaggle.com/datasets/marlesson/news-of-the-site-folhauol

The dataset includes the article titles, article URLs, full article text, and category. The news articles were collected from the Folha de São Paulo website: http://www.folha.uol.com.br/ between January 2015 and September 2017. Database Author WebScrapy Repository: https://github.com/marlesson/scrapy_folha

#### Steps

1. Vocabulary analysis and Word2Vec
2. News category classification with news tokenization and deep learning model
3. Improvement with transfer learning and GloVe

