# Week 14 Update

## Project Progress

So far, I have my dataset, basic coding, and visualizations ready for my final project. Right now, most of the dataset only reflects my own ChatGPT usage data, so I’m planning to expand the project by collecting data from a few other students with different majors to compare patterns across fields of study. I already requested datasets from friends majoring in biology, economics, and physics-math.  

I’m also continuing to explore whether there are additional interesting features or insights hidden in ChatGPT conversation data that I can analyze further.

---

## New Technique / Learning Process

One of the new techniques I researched during this project was how to process raw ChatGPT conversation archive data into a clean and structured dataset. At the beginning, I struggled because the raw JSON files contained many nested layers of information that were difficult to organize.

To learn this, I:
- Talked with Prof. WB
- Reviewed web articles
- Looked through Reddit discussions
- Revisited our earlier class materials on JSON files and data structures

Through this process, I learned how to loop through conversations and message nodes to extract useful information such as:
- Conversation IDs
- Sender roles
- Timestamps
- Message content

I also learned how to filter out unnecessary or incomplete data, such as:
- System messages
- Empty messages
- Messages without timestamps

Eventually, I was able to create a clean structured DataFrame called `messages_df` for analysis.

### Helpful Resources
- Reddit discussion on ChatGPT JSON archives:  
  https://www.reddit.com/r/OpenAI/comments/1i414z4/any_tips_on_making_json_conversation_archive/ 

- ConvoViz GitHub project:  
  https://github.com/mohamed-chs/convoviz#readme 

---

## Communication Strategy

For my presentation and communication strategy, I want to organize the narrative so the audience can easily follow along and stay engaged. During the warm-up activity we did in class, I noticed that presentations with strong visual elements and clear storytelling were the easiest to focus on and interact with.

Because of that, I plan to:
1. Begin with the most visually interesting graph or visualization to immediately introduce the main idea of the project
2. Move from broader trends into more detailed analyses

The presentation flow will likely look like this:
- Overall ChatGPT usage over time
- Usage by hour
- Heatmaps
- Correlation between prompt length and response length
- Comparisons across different majors

I’m planning to present using slides rather than only presenting directly from my website. Inspired by the interactive websites we looked at in class, I also want to incorporate small animations and smooth transitions to make the presentation more engaging and easier to follow.

