# Few-Shot Prompting for E-commerce Requirement Analysis – Comprehensive Report with Experiments, Pipeline, and Visualizations

![GenI-Banner](https://github.com/genilab-fau/genial-fau.github.io/blob/8f1a2d3523f879e1082918c7bba19553cb6e7212/images/geni-lab-banner.png?raw=true)

* Authors: [Michael Wanek](http://www.github.com/mwanek)
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

---

# Research Question 
How can few-shot prompting enhance requirement analysis for e-commerce platforms by providing accurate and context-aware feature specifications through experiments with varied parameters and a robust pipeline?

## Arguments
**What is already known about this topic:** Few-shot prompting is widely recognized for its ability to tailor AI responses to specific domains, including e-commerce. Prior research highlights its utility in automating various tasks, such as generating summaries and drafting content. However, challenges persist in maintaining accurate context across multiple prompts, especially when scaling complex software requirements. Existing literature emphasizes the importance of structured prompt design and parameter tuning to achieve reliable results in specialized fields.

**What this research is exploring:** This project explores how few-shot prompting with LLaMA 2/3 models can enhance e-commerce requirement analysis by examining the impact of different prompt templates and parameter settings. Using Ollama as the integration framework, we designed a Requirement Analysis Assistant that adapts dynamically to user inputs. The experiments aimed to identify optimal parameters that produce detailed, context-aware requirement specifications efficiently.

**Implications for practice:** This research demonstrates that integrating few-shot prompting into the requirement analysis phase can reduce manual effort, enhance accuracy, and accelerate project timelines. By experimenting with various prompt designs and model parameters, we provide practical insights for software analysts and developers. The findings suggest that well-engineered prompts can generate high-quality initial requirement drafts, freeing up time for in-depth analysis and stakeholder engagement.

# Research Method
**Experiment Design:** The study employed a systematic experimental design involving three sets of tests with varied parameters: `temperature` (0.5, 0.7, 0.9), `num_ctx` (100, 150, 200), and `num_predict` (100, 150, 200). A Python-based pipeline automated the process, sending API requests to the Ollama server, capturing JSON responses, and measuring response times. Each experiment was repeated multiple times to ensure reliability.

**Observations:** Experiments revealed that lower `temperature` values resulted in more deterministic outputs, ideal for generating consistent requirement specifications. Higher `num_ctx` settings allowed the model to retain more context from the few-shot examples, enhancing the coherence of complex requirements. Increasing `num_predict` extended the generated content, providing detailed technical solutions but also increasing response times.

**Results and Analysis:** The experiments produced diverse outputs, including database schema designs, API endpoint specifications, and secure transaction handling mechanisms. Response times ranged from 3.4 to 4.5 seconds, with longer response times observed in more complex prompts. Graphical visualizations highlighted trends, such as increased `num_predict` leading to richer outputs but higher latency. The analysis underscored the importance of balancing parameter settings to meet project needs.

**Conclusions:** The findings confirm that few-shot prompting can significantly enhance e-commerce requirement analysis, provided that prompt design and parameter tuning are carefully managed. The research underscores the potential of LLMs in automating initial requirement gathering, with visualizations offering a clear representation of the trade-offs between output quality and performance.

# Further Research
Future research could explore integrating feedback loops where user reviews refine prompts iteratively. Investigating multi-shot prompting and its impact on requirement analysis accuracy would be valuable. Additionally, integrating few-shot prompting with agile project management tools could enhance collaborative software development workflows, making AI-driven requirement analysis more dynamic and responsive to evolving project needs.
