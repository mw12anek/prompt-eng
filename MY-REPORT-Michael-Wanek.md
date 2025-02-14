![GenI-Banner](https://github.com/genilab-fau/genial-fau.github.io/blob/8f1a2d3523f879e1082918c7bba19553cb6e7212/images/geni-lab-banner.png?raw=true)

# Few-Shot Prompting for E-commerce Requirement Analysis

Using Few-Shot Prompting to extract and refine e-commerce platform requirements.

* Authors: [Michael Wanek](http://www.github.com/mwanek)
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

---

# Research Question 

How can few-shot prompting enhance requirement analysis for e-commerce platforms by providing accurate and context-aware feature specifications?

## Arguments

#### What is already known about this topic

* Few-shot prompting helps tailor AI responses for specific domains.
* Challenges include ensuring the context is accurately maintained across prompts.
* Possibility of automating initial requirement analysis phases using LLMs.

#### What this research is exploring

* We employ few-shot prompting with LLaMA 2 models.
* We are building a Requirement Analysis Assistant for e-commerce.
* We are exploring how to refine platform requirements from user inputs using LLMs.

#### Implications for practice

* It will be easier to generate initial requirement drafts.
* It will optimize time spent on early requirement gathering.
* We will better understand AI’s role in software development lifecycles.

# Research Method

This project uses Python-based few-shot prompting with the Ollama framework and LLaMA 2 models, integrated through a Jupyter Notebook (`few_shots.ipynb`).

Steps:
- Set up local Ollama server.
- Develop few-shot prompt examples.
- Integrate prompts into e-commerce scenarios.
- Evaluate output for accuracy and completeness.

# Results

Initial results show that few-shot prompts generate comprehensive and context-aware e-commerce requirements, such as order history and secure payment features.

# Further research

Future research could explore multi-shot prompting, integration with agile tools, and user feedback loops for continuous requirement refinement.
