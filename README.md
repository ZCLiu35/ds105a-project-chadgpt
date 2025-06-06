[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/WKKzpWVj)  
# Project ChadGPT  
## Description  
Our project focuses on exploring and analysing recipes from r/recipes to assist readers in cooking delicious yet nutritious meals. We aim to provide valuable insights and recommendations for navigating through the multitude of available recipes. 

### Key Features:  
- Exploration of recipes sourced from r/recipes along with nutrition data from BBC Good Food
- Investigation of the relationship between recipe popularity and nutritional content
- Data-driven recommendations for nutritious meals  

## 📚 Preparation  
If you want to replicate the analysis in this notebook, you will need to:    
1. Clone this repository to your computer 
2. Add it to your VSCode workspace 
3. Create a Reddit developer account and take note of your credentials (Reddit username, Reddit password, client ID, client secret) 
4. Create an OpenAI developer account and take note of your API key. This requires approximately $3 in GPT-3.5-turbo tokens.
5. Create a plain text file called `credentials.json` and add your Reddit credentials there:  

    ```json
    {
        "reddit_username": "<your Reddit username>",
        "reddit_password": "<your Reddit password>",
        "app_client_id": "<your Reddit app's client ID>",
        "app_client_secret": "<your Reddit app's client secret>",
        "openai_api_key": "<your OpenAI API key>"
    }
    ```
6. Use the `requirements.txt` file provided in this repository to install the required packages: 
    ```bash
    pip install -r requirements.txt
    ```

7. Run each noteboook in order of numbering.

8. Install R.

9. Install the required dependencies with the following code:
    ```r
    install.packages("ggplot2")
    install.packages("tidyverse")
    install.packages("ggradar")
    ```

10. Go to the `scripts` folder and run  `radar_plots.r`.

### Generative AI acknowledgement
- We wrote the notebooks in this repository on VSCode with GitHub Copilot extension activated. For code, we usually let Copilot autocomplete the code, check if it is correct and run the code to see if it accomplishes what we want. 
- We used ChatGPT by giving specific prompts to help us generate ideas on how to proceed. We also used it to help with finding errors in our code.
    - ChatGPT played a significant role in familiarizing us with the appropriate functions, in addition to consulting official documentation extensively. It was utilized both for debugging purposes and to inspire new ideas.
    - Example of use of ChatGPT 
        - Learn interactive plotting using Altair. An example plot could be: "Can you provide a brief overview of how to create interactive plots using Altair in Python?" ChatGPT will then generate a response that outlines the steps involved in creating interactive plots with Altair, explaining concepts such as encoding data, specifying chart types, and adding interactivity features like tooltips and selection. It was incredibly helpful in giving us ideas for our visualisations, such as using radar charts, frequency tables, histograms and more for our plots.
        - Brainstorming comparisons we can do using nutritional values and ingredients. Prompt: "What are some potential comparisons we can make using nutritional values and ingredients data?" ChatGPT could then generate ideas such as comparing the nutritional profiles of different cuisines, analyzing the most common ingredients used."
        - Additionally, we asked ChatGPT for specific methods we can use to filter out non-English posts. It provided us with various options such as regex, langid, and spacy, along with their respective pros and cons. This allowed us to gain a broad overview of our project, guiding our next steps. We then supplemented this knowledge by learning from the official documentation.