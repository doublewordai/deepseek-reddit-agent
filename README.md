## Reddit GenAI Trend Analysis with ReAct Agent Framework

Author: Amanda Milberg, Principal Solutions Engineer @ Doubleword

[Presentation Slides](https://docs.google.com/presentation/d/1nar6_2VrRtR7l6HcanoUFAql9l8THs3Ob6LT2PCbYGw/edit?usp=sharing)

🎯 **Main Purpose**:
- Analyzes r/technology subreddit posts to identify and summarize GenAI-related content
- Generates professional summaries of AI trends and developments to send to downstream users who want to stay up to date on the latest trends

🔑 **Key Components**:
1. Reddit API Integration to scrape relevant posts in a given subreddit (e.g. r/technology)
2. LLM-powered analysis to:
   - Determine GenAI relevance based on the thread title
   - Summarize key themes and content for each article
   - Generate trend analysis summary reports for all the GenAI related articles 

📊 **Process Flow**:
1. Fetches hot posts from r/technology 
2. Filters for GenAI-related content
3. Extracts and summarizes article content
4. Creates comprehensive trend analysis
5. Generates formatted report with sources ready to email to downstream users 

🛠️ **Technologies Used**:
- PRAW (Reddit API)
- OpenAI API/Self-hosted LLM
- BeautifulSoup for web scraping
- Markdown for report formatting
- ReAct agent framework

_Note: Requires Reddit API credentials and access to a LLM to function._

## Why Use an Agent Framework?
- Implements the ReAct (Reasoning + Acting) paradigm for more transparent and controlled AI behavior
- Provides explicit thinking and action steps for complex tasks
- Enables better debugging and monitoring of the AI's decision process

🧠 **ReAct Framework Benefits**:
1. **Reasoning Transparency**
   - Agent explicitly shows its thinking process before actions
   - Helps track decision-making logic
   - Makes debugging easier

2. **Structured Actions**
   - Clear separation between thinking and execution
   - Each action has defined inputs and outputs
   - Better error handling and recovery

3. **Process Monitoring**
   - Logs each step of the analysis pipeline
   - Tracks success/failure of individual components
   - Maintains history of decisions and actions

_The agent framework transforms what could be a simple script into a more robust, observable, and maintainable system for AI analysis. The agent approach provides better structure, transparency, and reliability for complex AI tasks compared to a simple main function._

## Why Self-Host?
🌟 **Key Benefits of Self-Hosting** 

1. **Cost-Effective Performance**
   - Reduced operational costs for high-volume processing
   - No ongoing API fees or usage limits

2. **Privacy & Data Control** 
   - Complete control over data processing and storage
   - No data sharing with external providers
   - Compliance with internal security policies
   - Ability to air-gap for sensitive applications & sensitive data 

3. **Deployment Flexibility**
   - Run locally on your own infrastructure
   - Scale resources based on actual needs

## Why Deep Seek?
1. **Specialized Reasoning Capabilities**
   - Optimized for logical reasoning and analysis tasks
   - Efficient chain-of-thought processing
   - Ideal for structured analytical workflows
2. **Open Source Technology + Self-Hosting Stack = 😍**  
   - Deepseek broke the internet 
   - Firm believer in owning your AI stack 
   - Smaller / specalized models for a given application  

_Note: In this demo we are running a self-hosted [DeepSeek-R1-Distill-Llama-8B](https://huggingface.co/deepseek-ai/DeepSeek-R1-Distill-Llama-8B) deployed on 4xL4 GPUs using [Doubleword's Infernece Platform](https://docs.doubleword.ai/). If you want to try this on your own you can pull this repository and swap in an OpenAI model. The code uses OpenAI compatiable endpoints so any model should be able to be swapped in. If you have any questions please reach out to: amanda.milberg@doubleword.ai_

