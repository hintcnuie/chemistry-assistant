# An AI teaching assistant for K12 chemistry

In the 2017-2018 school year, over 150,000 middle school STEM teacher positions were unfilled in public school systems across the US. The science teacher shortage has reached crisis level since the pandemic with unfilled positions in 50% of the school districts across the nation. The emergence of LLMs provides a potential solution to tailor personalized STEM education to each student. Yet, ChatGPT is too expensive, lacks privacy, and most importantly, often hallucinates and confuses facts from different domains. 

In this project, I created a "chemistry teaching assistant" AI agent. The application supplements user questions (ie, prompts) with context from an RAG vector database of facts about chemical elements. It could use a plain Llama2 or a finetuned LLM to generate answers from the context. The finetuned model is developed with 1700+ pairs of questions and answers I generated on the subject of chemistry elements. It helps the model "understand" the chemistry vocabulary and focus on the domain subject to reduce hallucination -- e.g. it no longer confuses facts from Mercury the planet with Mercury the element. 

I further built a Discord bot to make the teaching assistant available in Discord, which is very popular among my peer middle school students. You can [join the Discord server](https://discord.gg/EuCkCNKu8c) and chat with the teaching assistant bot yourself or [add it to your own server](https://discord.com/oauth2/authorize?client_id=1213953089208320030&permissions=8&scope=bot)!

Or, you can [try it on the web](https://0xb409673c9a640429c7e10ed24aa6e0bdcf1bbe41.gaianet.xyz/).

In this repo, I provide open-source code and instructions on how I created this AI assistant.

[Step 1: create a chemistry knowledge base for RAG](rag-embeddings/)

[Step 2: finetune an open-source LLM for the chemistry subject](fine-tune-model/)

[Step 3: Deploy an API server](api-server/)

[Step 4: Create the Discord bot](discord/)


