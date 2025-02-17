# Few-Shot Prompting for E-commerce Requirement Analysis – Comprehensive Report with Experiments, Pipeline, and Visualizations

![GenI-Banner](https://github.com/genilab-fau/genial-fau.github.io/blob/8f1a2d3523f879e1082918c7bba19553cb6e7212/images/geni-lab-banner.png?raw=true)

* Authors: [Michael Wanek](http://www.github.com/mwanek)
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

---

# Research Question 
How can few-shot prompting enhance requirement analysis for e-commerce platforms by providing accurate and context-aware feature specifications through experiments with varied parameters and a robust pipeline?

## Arguments
**What is already known about this topic:** Few-shot prompting is widely recognized for its ability to tailor AI responses to specific domains, including e-commerce. Prior research highlights its utility in automating various tasks, such as generating summaries and drafting content. However, challenges persist in maintaining accurate context across multiple prompts, especially when scaling complex software requirements. Existing literature emphasizes the importance of structured prompt design and parameter tuning to achieve reliable results in specialized fields.

**What this research is exploring:** This project explores how few-shot prompting with LLaMA 2/3 models can enhance e-commerce requirement analysis by examining the impact of different prompt templates and parameter settings. Using Ollama as the integration framework, we designed a Requirement Analysis Assistant that adapts dynamically to user inputs. Experiments varied `temperature` to control randomness, `num_ctx` to manage context retention, and `num_predict` to determine output length. This ensured a comprehensive analysis of how each parameter influenced output quality, detail, and consistency.

**Implications for practice:** Integrating few-shot prompting into requirement analysis can significantly reduce manual effort, enhance accuracy, and speed up project timelines. The study demonstrated that lower `temperature` values produce deterministic results, higher `num_ctx` values improve context retention, and higher `num_predict` values generate detailed outputs. These findings provide practical insights for software analysts, emphasizing the importance of tuning model parameters for optimal performance.

# Research Method
**Experiment Design:** The experiments included three sets of parameter variations: `temperature` (0.5, 0.7, 0.9), `num_ctx` (100, 150, 200), and `num_predict` (100, 150, 200). Each combination affected the model's output differently. Lower `temperature` yielded consistent, stable outputs suitable for technical tasks, while higher values introduced creativity. Increased `num_ctx` preserved more details from few-shot examples, and higher `num_predict` produced more comprehensive responses. A Python pipeline automated the entire process, ensuring consistent API communication, response capture, and timing measurements.

**Results and Analysis:** The responses reflected the impact of parameter adjustments. For example, `temperature=0.5` with `num_ctx=200` and `num_predict=100` provided concise, coherent outputs, while `temperature=0.9` with `num_ctx=100` and `num_predict=200` generated more detailed but less consistent results. Response times ranged from ~3.4s to ~4.5s, with higher `num_predict` values causing increased latency. Visualizations highlighted these patterns, emphasizing the trade-offs between output length, detail, and time.

**Conclusions:** The findings illustrate that careful tuning of `temperature`, `num_ctx`, and `num_predict` is essential for optimizing AI-generated requirement specifications. Lower temperatures are ideal for deterministic outputs, higher context values improve coherence, and increased predictions enhance detail at the cost of time. This study underscores the potential of LLMs in automating software requirement analysis, with visualizations offering clear insights into parameter impact.

# Further Research
Future research could explore integrating feedback loops where user reviews refine prompts iteratively. Investigating multi-shot prompting and its impact on requirement analysis accuracy would be valuable. Additionally, integrating few-shot prompting with agile project management tools could enhance collaborative software development workflows, making AI-driven requirement analysis more dynamic and responsive to evolving project needs.
