# prose-genie
Use this application as a basis for your writing content or to test out the unhinged nature of the [GPT-2 language model](https://openai.com/index/better-language-models/). This project is built on Flask, a web framework that can be used to build web applications that utilize Python. 

## Demonstration

https://github.com/snehasad/prompt-genie/assets/104543929/a741fb3b-eb76-470d-82b1-aa62d64fcebb
## Getting Started
### Installation Requirements
  * [Python 3.7+](https://www.python.org/)
  * [PyTorch](https://pytorch.org/)
  * [Hugging Face - Transformers](https://huggingface.co/docs/transformers/en/index) (You will use this to load the GPT-2 pre-trained model)
  * [Flask](https://flask.palletsprojects.com/en/3.0.x/)

### Installation Instructions
  1. Install PyTorch (CPU only, change command if you need GPU support)
        ```sh
      pip install torch
      ```
  2. Install Hugging Face Transformers
     ```sh
      pip install transformers
      ```
  3. Install Flask
     ```sh
      pip install Flask
      ```
  4. Install additional Hugging Face libraries for dataset handling and data collating
     ```sh
      pip install datasets
      ```
## Usage
Once installation is complete, you may proceed to copy my code from `newapp.py` and `essays.txt`. I included the HTML script in `newapp.py`, so you won’t need an index.html file for this project. 

You can run the app in development mode by pasting the following command in your terminal:
```sh
 python3 newapp.py
```

You should see your code running at [http://127.0.0.1:5000/](http://127.0.0.1:5000/). Refresh the page to test a different prompt.

Now you can modify `newapp.py`. To view the modified changes, **ctrl + s** `newapp.py`, then refresh your browser. This will trigger the Flask debugger to restart.
### Additional Notes  
GPT-2 works by predicting the next word, given on all the previous words within your prompt. To generate more coherent and relevant text, try structuring your prompt as a narrative rather than as a command. For example, instead of saying ***"Tell me about (topic),"*** you could start with ***"Today, I learned about (topic)."*** 
      
