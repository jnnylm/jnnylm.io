# Week 11 Update

---
## Data Source Selection

For my final project, I chose to work with my personal ChatGPT usage data. I selected this dataset because it directly reflects my own study habits, workflow, and interaction patterns with AI tools. Since I frequently use ChatGPT for a variety of tasks, analyzing this data allows me to explore meaningful behavioral trends over time.

---
## Data Acquisition

I successfully obtained my dataset by requesting my data through the ChatGPT platform. The data was provided in a JSON format, containing a full history of my interactions.

---
## Motivation and Provenance

This dataset was originally created by OpenAI as part of the normal operation of the ChatGPT system to support and improve user interactions. It was not designed for a specific research purpose or academic study.

Key provenance considerations:
- The data is automatically generated during real-time use
- No manual input or curation was involved in its collection
- It reflects system-logged interactions rather than intentional data design
- It is maintained by OpenAI

Because of this, the dataset is highly authentic but not structured for analysis.

---
## Composition of the Dataset

The dataset represents a complete record of my ChatGPT interactions rather than a sample. However, it is still limited in scope because it only captures AI-assisted activities.

Important characteristics:
- Contains multiple conversations with nested message structures
- Includes timestamps for each interaction
- Stores both user prompts and system responses
- Data is stored in JSON format, not a flat table

Limitations in composition:
- Missing context behind why prompts were written
- No predefined labels for task types
- Possible redundancy from repeated prompts
- Some conversations may be incomplete or fragmented

---
## Appropriate and Inappropriate Uses

Appropriate uses:
- Personal behavioral analysis
- Time-series analysis of usage patterns
- Understanding interaction frequency and habits

Inappropriate uses:
- Generalizing findings to all ChatGPT users
- Making objective judgments about productivity or performance

---
## Preliminary Exploratory Analysis

During initial exploration in Google Colab, I observed:

- The dataset has a nested JSON structure, requiring transformation before analysis
- Each conversation contains multiple back-and-forth messages
- Message content is inconsistent (plain text vs structured objects)
- Each message includes a timestamp, enabling time-based analysis

These findings confirmed that preprocessing will be a critical step before meaningful analysis can begin.

---
## Data Cleaning and Wrangling

### What I Have Done So Far:
- Imported the JSON dataset into Google Colab
- Explored the structure of the data
- Identified relevant fields (e.g., message content, timestamps)

### What Still Needs to Be Done:
- Flatten the nested JSON structure into a tabular format
- Remove irrelevant or empty entries
- Drop unnecessary columns
- Convert Unix timestamps into readable datetime format

### New Features to Create:
- Prompt length (word count and character count)
- Time-based features (hour of day, day of week)
- Session grouping (based on time gaps between messages)
- Prompt categorization (e.g., coding, writing, brainstorming)

---
## Strengths and Limitations

### Strengths:
- Highly personalized and relevant dataset
- Captures real-world usage behavior
- Includes both quantitative (timestamps, counts) and qualitative (text) data

### Limitations:
- Requires subjective interpretation for categorization
- Lacks explicit context or intent behind prompts
- Only reflects AI-assisted work, not overall productivity

---
## Challenges and Roadblocks

One of the main challenges I encountered is the complexity of the dataset structure. Unlike CSV files with clearly defined columns, this dataset is deeply nested, making it difficult to interpret and organize.

Specific challenges include:
- Identifying what constitutes a single “session”
- Flattening the JSON structure into usable rows
- Handling large text fields efficiently
- Dealing with inconsistent message formats

These issues have made the preprocessing stage more time-consuming than expected.

---
## Summary

Overall, I successfully selected and obtained my dataset and began preliminary exploration. I identified key structural challenges and outlined the necessary steps for cleaning and feature engineering. Moving forward, my main focus will be transforming the data into a usable format and creating meaningful features for analysis.
