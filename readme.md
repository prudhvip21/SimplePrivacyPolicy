# Simple Privacy Policy (SiPP)

Privacy policies are long and hard to read. SiPP summarises a privacy policy into the practices that matter to users, such as what data is collected, who it is shared with, how long it is kept and what control the user has.

## How it works

- Policy text is split into segments and classified into OPP-115 privacy practice categories: First Party Collection/Use, Third Party Sharing/Collection, Data Retention, Data Security, User Access, Edit and Deletion, and User Choice/Control
- Supervised models built with BERT through Hugging Face Transformers and PyTorch, alongside unsupervised approaches
- A Flask web app where a user submits a policy and sees the summary by category

## Run it

```
pip install -r requirements.txt
python3 app.py
```

`requirements.txt` lists the web app dependencies. The modelling code in `model_impl/` and `pyFiles/` also uses PyTorch, Transformers, NLTK, spaCy and Gensim.

## Repository layout

- `app.py`, `sipp_app.py`: Flask app
- `templates/`, `static/`: web pages
- `model_impl/`, `pyFiles/`: modelling code
- `data/`, `OPP-115/`: the OPP-115 corpus and model outputs
- `privary_policy_text/`, `test_data/`: sample policies
- `Code_archive/`: earlier versions of the code

## Data

Uses the OPP-115 corpus of annotated website privacy policies (Wilson et al., 2016, Usable Privacy Policy Project). Credit for the corpus remains with its authors; check its terms before reuse.

## Team

Built by Prudhvi Potuganti with [dhiraj-v](https://github.com/dhiraj-v), [IssacBala](https://github.com/IssacBala) and [manoj-sirvi](https://github.com/manoj-sirvi). The commit history from the original team repository is preserved here.
