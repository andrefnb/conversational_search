# conversational_search

Master's Degree in Big Data analysis and engeneering. Information Retrieval course's project.

Motivation

Conversational Information Seeking (CIS) is highlighted as an important emerging research area in the SWIRL
2018 workshop report on future trends in Information Retrieval. CIS is timely and important with increased
adoption of a new generation of conversational ‘assistant' systems, including Amazon Alexa, Cortana, Bixby,
Google Assistant, and many others. Voice-based assistant interactions are now common, with a recent Comscore
report showing that over 20% of homes in America own a smart speaker and over 500M devices with the Google
Assistant worldwide. However, despite current assistants' ability to perform simple well-defined actions, their
ability to support conversational information seeking is still very limited.

The goal of this TREC track is to pursue CIS research and create a large-scale reusable test collections for open-
domain conversational search systems. The primary initial focus will be on system understanding of information
needs in a conversational format and finding relevant responses using contextual information. In particular, we
are motivated by long-running and complex tasks requiring multiple turns (possibly multiple sessions). The figure
to the right shows a typical pipeline for a conversational agent system. The vision is to address all of these
aspects. We first focus on retrieval of relevant result content in context.

Dataset
MS MARCO web passage data
• MS MARCO Passage Reranking data;
• 10 million answer candidates from Bing search;
• This data is publicly available.

Implementation steps:
• Retrieval;
• Embeddings
• Ranking
• Conversation tracking

Implementation:
• An ElasticSearch service will be available to search the corpus;
• A BERT service with Google’s pre-trained model will be available to create sentence embeddings;
• Learning to rank through a logistic regression classifier that uses as training set the pairs of questions and passages, with their respective relevance judgments provided in TRECCASTeval;
• Information retrieval algorithms (LMD, RM3, etc), featuring expanded queries and historical query expansion;
• Performance analysis using predefined metrics.
