# Task 3: Fake News Detection

This repository contains the _dataset_, _format checker, scorer and baselines_ for the [CLEF2021-CheckThat! Task 3](https://sites.google.com/view/clef2021-checkthat/tasks/task-3-fake-news-detection). 
Given the text of a news article, determine whether the claims made in the article are true, partially true, false or other (e.g., claims in dispute) and also detect the topical domain of the article. This task will run in English.

This file contains the basic information regarding the CLEF2021-CheckThat! Task 3
on check-worthiness on tweets provided for the CLEF2021-CheckThat! Lab
on "Automatic Detecting Check-Worthy Claims, Previously Fact-Checked Claims, and Fake News".
The current version (?) corresponds to the release of the first batch of the training data set. 
The test set is released with the current version.


__Table of contents:__
- [Evaluation Results](#evaluation-results)
- [List of Versions](#list-of-versions)
- [Contents of the Task 3 Directory](#contents-of-the-repository)
- [Input Data Format](#input-data-format)
	- [Subtask 3A: Multi-Class Fake News Detection of News Articles](#Subtask-3A-Multi-Class-Fake-News-Detection-of-News-Articles)
	- [Subtask 3B: Topical Domain Classification of News Articles](#Subtask-3B-Topical-Domain-Classification-of-News-Articles)
- [Output Data Format](#output-data-format)
	- [Subtask 3A: Multi-Class Fake News Detection of News Articles](#Subtask-3A-Multi-Class-Fake-News-Detection-of-News-Articles-1)
	- [Subtask 3B: Topical Domain Classification of News Articles](#Subtask-3B-Topical-Domain-Classification-of-News-Articles-1)
- [Format Checkers](#format-checkers)
	- [Subtask 3A: Multi-Class Fake News Detection of News Articles](#Subtask-3A-Multi-Class-Fake-News-Detection-of-News-Articles-2)
	- [Subtask 3B: Topical Domain Classification of News Articles](#Subtask-3B-Topical-Domain-Classification-of-News-Articles-2)
- [Scorers](#scorers)
	- [Subtask 3A: Multi-Class Fake News Detection of News Articles](#Subtask-3A-Multi-Class-Fake-News-Detection-of-News-Articles-3)
	- [Subtask 3B: Topical Domain Classification of News Articles](#Subtask-3B-Topical-Domain-Classification-of-News-Articles-3)
- [Evaluation Metrics](#evaluation-metrics)
- [Baselines](#baselines)
	- [Subtask 3A: Multi-Class Fake News Detection of News Articles](#Subtask-3A-Multi-Class-Fake-News-Detection-of-News-Articles-4)
	- [Subtask 3B: Topical Domain Classification of News Articles](#Subtask-3B-Topical-Domain-Classification-of-News-Articles-4)
- [Credits](#credits)

## Evaluation Results

TBA

## List of Versions

- **subtask-3a--english-v1.0 [2021/04/06]** - Sample data for task 3a is relaeased, consisting 50 news article. (Released)
- **subtask-3a--english-v1.0 [2021/04/15]** - 2nd batch of data will be released (scheduled)

## Contents of the Task 3 Directory
We provide the following files:

- Main folder: [data](./data)
  - subfolder: subtask-3A--english
  - subfolder: subtask-3B--english
- Main folder: [baseline](./baseline)<br/>
- 	Contains scripts provided for baseline models of the tasks
- Main folder: [baseline](./format_checker)<br/>
- 	Contains scripts provided to check format of the submission file
- Main folder: [baseline](./scorer)<br/>
- 	Contains scripts provided to score output of the model when provided with label (i.e., dev set).
- [README.md](./README.md) <br/>
- 	This file!



## Input Data Format

The data will be provided in the format of Id, title, text, rating, domain the description of column are as follows:

- ID- Unique indetifier of the news article
- Title- Title of the news article
- text- Text mentioned inside the news article
- rating - class of the news article as false, partially false, true, other
- domain - domain of the given news article(applicable only for task B)

### Subtask 3A: Multi-Class Fake News Detection of News Articles

Subtask 3A: Multi-class fake news detection of news articles (English): Sub-task A would be the detection of fake news designed as a four-class classification problem. The training data will be released in batches and will be roughly about 1,000 articles with the respective label. Given the text of a news article, determine whether the main claim made in the article is true, partially true, false, or other. 

### Topical Domain Classification of News Articles

Subtask 3B: Fact-checkers require background expertise to identify the truthfulness of an article. The categorisation will help to automate the sampling process from a stream of data. Given the text of a news article, determine the topical domain of the article (English). This is a classification problem. The task is to categorise fake news articles into five or more different topical categories like health, election, conspiracy theory etc. This task will be offered for a subset of the data of Subtask 3A.

## Output Data Format

### Subtask 3A: Multi-Class Fake News Detection of News Articles

We need the output file in the format of Id, rating.

### Topical Domain Classification of News Articles

We need the output file in the format of Id, domain.


## Format Checkers

#### Subtask 3A: Multi-Class Fake News Detection of News Articles

TBA

#### Topical Domain Classification of News Articles

TBA

## Scorers

### Subtask 3A: Multi-Class Fake News Detection of News Articles

TBA

### Topical Domain Classification of News Articles

TBA

## Evaluation Metrics
This task is evaluated as a classification task. We will use the F1-macro measure for the ranking of teams.


## Baselines

### Subtask 3A: Multi-Class Fake News Detection of News Articles

TBA

### Topical Domain Classification of News Articles

TBA


## Credits

Task 3 Organizers: 

- Thomas Mandl, University of Hildesheim
- Julia Maria Struß, University of Applied Sciences Potsdam
- Gautam Kishore Shahi, University of Duisburg-Essen
- Sandip Modha, LDRP Institute of Technology and Research

Task website: https://sites.google.com/view/clef2021-checkthat/tasks/task-3-fake-news-detection

Contact:   clef-factcheck@googlegroups.com
