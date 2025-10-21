# Tokenization

Author: Youssef Al Hariri

This repository explains and simplifies the concept of tokenization in text processing and LLM modeling using various methods and libraries. Contributions and feedback are welcome.

## Exercises

You can access four notebooks:

1. [**Basic Tokenization**](/notebooks/tokenization_1.ipynb) 
   A survey of different tokenization methods. It ends with an interactive tool to compare how different libraries and methods handle tokenization.


2. [**Tiktoken Example**](/notebooks/tokenization_2.ipynb)
   A focused example that demonstrates tokenization using the tiktoken library (a fast BPE tokenizer by OpenAI).


3. [**Notebook 12.3: Tokenization**](/notebooks/12_3_Tokenization.ipynb) 
   A modified copy of the notebook "12_3_Tokenization" from the book _Understanding Deep Learning_.

4. [**Training a Tokenizer model**](/notebooks/training_tokenizer/tokenization_3_training.ipynb)
   A simple example to build a tokenizer model by using a simple training data.
   
## Extra reading
- Articles:
  - M. Schuster and K. Nakajima. 2012. Japanese and Korean voice search. IEEE. https://doi.org/10.1109/ICASSP.2012.6289079
  - Rico Sennrich, Barry Haddow, and Alexandra Birch. 2016. Neural Machine Translation of Rare Words with Subword Units. ACL. https://aclanthology.org/P16-1162/
  - Taku Kudo. 2018. Subword Regularization: Improving Neural Network Translation Models with Multiple Subword Candidates. ACL. https://aclanthology.org/P18-1007/

- Books:
  - Prince, Simon J.D. _Understanding Deep Learning_. MIT Press, 2023. (see chapters on tokenization)

## Getting started with the practices

These notebooks were developed with standard Python tooling. The steps below will get a local environment ready to run the notebooks (Python 3.11.5 was used).

1. Create and activate a virtual environment (recommended):

   - macOS / Linux (zsh/bash):

     python3 -m venv .venv
     source .venv/bin/activate

   - Windows:

     python -m venv .venv
     .\\.venv\\Scripts\\activate

2. Install dependencies

   ```shell
   pip install -r requirements.txt
   ```

3. Open the notebooks within VS Code, OR launch Jupyter Lab and open the notebooks folder:

   ```shell
   jupyter lab
   ```

Notes
- If a `requirements.txt` file is added to the repository, prefer using it to reproduce the exact environment.
- If a notebook fails to open due to a missing package, install the missing package into the activated virtual environment and refresh the notebook page.

- _Optional_: 

A. small spaCy model must be downloaded separately after installing spaCy:
```shell
python -m spacy download en_core_web_sm
```

B. NLTK data (punkt) may need to be downloaded at runtime:
```shell
python -c "import nltk; nltk.download('punkt')"
```

Contributions and issues are welcome — please open a GitHub issue or submit a pull request with suggested changes.


---

NOTICE

This repository contains notebooks adapted from external sources (for
example: material adapted from Simon J.D. Prince's "Understanding Deep
Learning"). The Apache-2.0 license applied here covers original code
and content added to this repository by the copyright holder. It does
not change or override the copyright or license terms of third-party
works that may be included in or referenced by the notebooks. If any
third-party content in the notebooks has a more restrictive license or
requires explicit permission to redistribute, users should contact the
original copyright holder before redistributing that content.
