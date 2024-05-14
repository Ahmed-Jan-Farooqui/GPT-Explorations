# GPT-Explorations
A collection of notebooks and scripts exploring OpenAI API and LangChain Agentic workflows.
## The Notebooks
I made a few notebooks exploring the possibilities of the OpenAI API towards the end of developing a capable data science chatbot. I wanted to explore how well it could handle Exploratory Data Analysis (EDA) questions, Basic Inference (using classical machine learning techniques), and Super Inference (using modern machine learning techniques). For this, I made three notebooks experimenting with:
<ol>
  <li>
    Built-in Agents from LangChain for EDA and basic inference.
  </li>
  <li>
    Custom Agent for EDA and basic inference.
  </li>
  <li>
    Custom and LangChain built-in agent for Super Inference
  </li>
</ol>
## The Scripts
Using the lessons learned from the notebooks, I made two scripts for deployment in an end-to-end application. These scripts provide the functions necessary to run the Agents in a production environment. I made one script for the EDA and Basic Inference agent and one for the Super Inference agent. Some interesting observations:
<ol>
  <li>I found that the Python Repl Tool that LangChain provides was too unreliable in producing deterministic code for some reason, so I chose to use subprocess spawning instead, whereby the LLM would output the code, and I would extract it and use it.</li>
  <li>I elected to specify the path to the .csv file in the investigation instead of trying to provide it directly, as that was not producing good results.</li>
</ol>
