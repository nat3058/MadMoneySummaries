# MadMoneySummaries
https://nat3058.github.io/MadMoneySummaries/

# About
A static site containing AI-generated bulleted summaries every weekday for the popular (Mon-Fri) financial show “Mad Money”. 

# Inspiration
As a ordinary citizen, I wanted to be more aware of what's been happening in the financial markets. 
I wanted this information to be straight to the point without too much fluff.
The CNBC TV show **Mad Money** seems to give new and unqiue information (especially the interviews with CEOs of different companies).
LLMs seem to be able to digest natural language and extract/present the right information in the right style. 

This website is the result of the two.  

# Features
▪ Python script does all the heavy lifting described below (not yet released in this repo, but I will if folks star this repo) 
▪ Data pipeline to gather and preprocess transcripts 
▪ Prompts AI to generate insightful, HTML-styled summaries using Llama3.1 LLM API 
▪ Adds new files containing new summaries to the website
▪ Mult-threaded to increase throughout if you want summaries for multiple epidodes at once
▪ Experimented with RAG (Retrieval-Augmented Generation) using LlamaIndex to enhance summary quality (but it acc reduced performance)

# Future
▪ **Zero-Trust:** Currently mitigating hallucination or any misinformation by adding verbatim transcript evidence & timestamp for each summary claim
▪ **Interactive Insights:** Would be cool if users could ask additional or followup questions regardign the summary info to the AI (such as Can you explain what this term means? or Give me more details regarding XYZ segement of the episode.)
▪ **Improve Summary Quality:** Experiment with different ways providing context/prompts, summarization methods, hyperparameters like chunk size, other methods like RAG, better preprocessing, other audio-to-text transcription techniques to improve transcrption quality, etc.
▪ **Summaries Sent Stright To Email Inbox:** Implement feature to allow users to sign up for emails with summaries of every new episode 
▪ More generally, clean up the python script code... perhaps refactor into a easy-to-use library to abstract information gathering/preprocessing methods 
▪ Host the website with a custom domain name
▪ Other shows?!? Shark Tank? Squak Box? Youtube Channels (Low Level Learning)!?!?