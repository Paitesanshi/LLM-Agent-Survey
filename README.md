# A Survey on LLM-based Autonomous Agents

Autonomous artificial intelligence (AI) agents are designed to accomplish specific objectives by self-guided instructions, automatic memorization, planning, and action. With the advent and prospering of large language models (LLMs), there is an expanding frontier in using LLMs as core controllers for these autonomous entities. However, a unified view that ties together the diverse studies in this field has been lacking. This repository houses a comprehensive and systematic survey that fills this gap, focusing on LLM-based autonomous AI agents in their construction, applications, and evaluation strategies.

In particular, we explore the essential components of an AI agent, including a profile module, a memory module, a planning module, and an action module. We further investigate the potential applications in natural and social sciences and introduce methods to evaluate their effectiveness. Challenges and future directions of this field are also discussed.

Our paper and this repository aim to serve as a resource for researchers and practitioners alike, providing insights, related references, and continuous updates on this exciting and rapidly evolving field.



## News
- [8/23/2023] The first version of the paper is released on arXiv: [A Survey on Large Language Model based Autonomous Agents](https://arxiv.org/abs/2308.11432)

## Table of Contents

- [A Survey on LLM-based Autonomous Agents](#a-survey-on-llm-based-autonomous-agents)
  - [News](#news)
  - [Table of Contents](#table-of-contents)
  - [Growth Trend of LLM-based Autonomous Agent](#growth-trend-of-llm-based-autonomous-agent)
  - [Structure of the Survey](#structure-of-the-survey)
  - [Construction of LLM-based Autonomous Agent](#construction-of-llm-based-autonomous-agent)
  - [Applications of LLM-based Autonomous Agent](#applications-of-llm-based-autonomous-agent)
  - [Evaluation on LLM-based Autonomous Agent](#evaluation-on-llm-based-autonomous-agent)
  - [More Comprehensive Summarization](#more-comprehensive-summarization)
  - [Maintainers](#maintainers)
  - [Citation](#citation)
  - [How to Contribute](#how-to-contribute)
  - [Acknowledgement](#acknowledgement)
  - [Contact Us](#contact-us)

## Growth Trend of LLM-based Autonomous Agent
![Growth Trend](assets/trend.png)
<hr>

## Structure of the Survey
![Structure](assets/survey.png)


## Construction of LLM-based Autonomous Agent
![Architecture Design](assets/architecture.png)
<table >
    <tr>
        <td rowspan='2'align='center'>Model</td>
        <td rowspan='2'align='center'>Profile</td>
        <td colspan='2'align='center'>Memory</td>
        <td rowspan='2'align='center'>Planning</td>
        <td rowspan='2'align='center'>Action</td>
        <td rowspan='2'align='center'>LS</td>
        <td rowspan='2'align='center'>Time</td>        
        <td rowspan='2'align='center'>Paper</td>
        <td rowspan='2'align='center'>Code</td>
    </tr>
    <tr>
        <td align='center'>Operation</td>
        <td align='center'>Structure</td>
    </tr>
    <tr>
        <td align='center'>WebGPT</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>Human feedback</td> 
        <td align='center'>12/2021</td>
        <td align='center'><a href="https://arxiv.org/abs/2112.09332">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>SayCan</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>Environment feedback</td>  
        <td align='center'>04/2022</td> 
        <td align='center'><a href="https://arxiv.org/abs/2204.01691">Paper</a></td>
        <td align='center'><a href="https://say-can.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MRKL</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td>  
        <td align='center'>05/2022</td> 
        <td align='center'><a href="https://arxiv.org/abs/2205.00445">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Inner Monologue</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>Environment feedback</td> 
        <td align='center'>07/2022</td> 
        <td align='center'><a href="https://arxiv.org/abs/2207.05608">Paper</a></td>
        <td align='center'><a href="https://innermonologue.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Social Simulacra</td>  
        <td align='center'>GPT-Generated</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>   
        <td align='center'>08/2022</td> 
        <td align='center'><a href="https://arxiv.org/abs/2208.04024">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ReAct</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>Environment feedback</td> 
        <td align='center'>10/2022</td> 
        <td align='center'><a href="https://arxiv.org/abs/2210.03629">Paper</a></td>
        <td align='center'><a href="https://github.com/ysymyth/ReAct">Code</a></td>
    </tr>
    <tr>
        <td align='center'>REPLUG</td> 
        <td align='center'>-</td>  
        <td align='center'>Read/Write/Reflection</td> 
        <td align='center'>Unified</td> 
        <td align='center'>-</td>  
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>  
        <td align='center'>01/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2301.12652">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>DEPS</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>Environment feedback</td> 
        <td align='center'>02/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2302.01560">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Toolformer</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>Example</td>  
        <td align='center'>02/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2302.04761">Paper</a></td>
        <td align='center'><a href="https://github.com/lucidrains/toolformer-pytorch">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Reflexion</td> 
        <td align='center'>-</td>  
        <td align='center'>Read/Write/Reflection</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>Environment feedback</td> 
        <td align='center'>03/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2303.11366">Paper</a></td>
        <td align='center'><a href="https://github.com/noahshinn024/reflexion">Code</a></td>
    </tr>
    <tr>
        <td align='center'>CAMEL</td> 
        <td align='center'>Handcrafting & GPT-Generated</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td>  
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>  
        <td align='center'>03/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2303.17660">Paper</a></td>
        <td align='center'><a href="https://github.com/camel-ai/camel">Code</a></td>
    </tr>
    <tr>
        <td align='center'>API-Bank</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td>  
        <td align='center'>w/ tools</td> 
        <td align='center'>Example</td> 
        <td align='center'>04/2023</td> 
        <td align='center'><a href="url">Paper</a></td>
        <td align='center'><a href="url">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ViperGPT</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ tools</td>  
        <td align='center'>-</td>  
        <td align='center'>03/2023</td>  
        <td align='center'><a href="https://arxiv.org/abs/2303.08128">Paper</a></td>
        <td align='center'><a href="https://github.com/cvlab-columbia/viper">Code</a></td>
    </tr>
    <tr>
        <td align='center'>HuggingGPT</td> 
        <td align='center'>-</td>  
        <td align='center'>Read/Write</td> 
        <td align='center'>Unified</td> 
        <td align='center'>w/o feedback</td>  
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td>  
        <td align='center'>03/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2303.17580">Paper</a></td>
        <td align='center'><a href="https://huggingface.co/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Generative Agents</td> 
        <td align='center'>Handcrafting</td> 
        <td align='center'>Read/Write/Reflection</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/o tools</td>  
        <td align='center'>-</td>  
        <td align='center'>04/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2304.03442">Paper</a></td>
        <td align='center'><a href="https://github.com/joonspk-research/generative_agents">Code</a></td>
    </tr>
    <tr>
        <td align='center'>LLM+P</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td>  
        <td align='center'>04/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2304.11477">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChemCrow</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>-</td> 
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.05376">Paper</a></td>
        <td align='center'><a href="https://github.com/ur-whitelab/chemcrow-public">Code</a></td>
    </tr>
    <tr>
        <td align='center'>OpenAGI</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>Example</td>
        <td align='center'>04/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/agiresearch/OpenAGI/blob/main/README.md">Code</a></td>
    </tr>
    <tr>
        <td align='center'>AutoGPT</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w feedback</td>
        <td align='center'>w tools</td>
        <td align='center'>Environment feedback</td> 
        <td align='center'>04/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/Significant-Gravitas/Auto-GPT">Code</a></td>
    </tr>
    <tr>
        <td align='center'>SCM</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>-</td> 
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.13343">Paper</a></td>
        <td align='center'><a href="https://github.com/wbbeyourself/scm4llms">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Socially Alignment</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>Example</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16960">Paper</a></td>
        <td align='center'><a href="https://github.com/agi-templar/Stable-Alignment">Code</a></td>
    </tr>
    <tr>
        <td align='center'>GITM</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>Environment feedback</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.17144">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenGVLab/GITM">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Voyager</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Unified</td>
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>Environment feedback</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16291">Paper</a></td>
        <td align='center'><a href="https://github.com/MineDojo/Voyager">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Introspective Tips</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Unified</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/o tools</td>
        <td align='center'>Example & Environment feedback</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.11598">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>RET-LLM</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Unified</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>Example</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.14322">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChatDB</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/Reflection</td> 
        <td align='center'>Unified</td> 
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td> 
        <td align='center'>06/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.03901">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>S3</td> 
        <td align='center'>Dataset alignment</td>
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Hybrid</td> 
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>-</td> 
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.14984">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChatDev</td>
        <td align='center'>Handcrafting</td>
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Unified</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/o tools</td>
        <td align='center'>-</td> 
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.07924">Paper</a></td>
        <td align='center'><a href="url">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ToolLLM</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td>
        <td align='center'>Example</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.16789">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ToolBench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MemoryBank</td> 
        <td align='center'>-</td> 
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>-</td> 
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.10250">Paper</a></td>
        <td align='center'><a href="https://github.com/zhongwanjun/MemoryBank-SiliconFriend">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MetaGPT</td>
        <td align='center'>Handcrafting</td>
        <td align='center'>Read/Write/Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>-</td>  
        <td align='center'>08/2023</td> 
        <td align='center'><a href="https://arxiv.org/abs/2308.00352">Paper</a></td>
        <td align='center'><a href="https://github.com/geekan/MetaGPT">Code</a></td>
    </tr>
</table>

*This table only summarizes partial previous work. See section [More comprehensive Summarization](#more-comprehensive-summarization) for more papers.*

## Applications of LLM-based Autonomous Agent

<table>
    <tr>
        <td align='center'>Title</td>
        <td align='center'>Social Science </td>
        <td align='center'>Natural Science </td>
        <td align='center'>Engineering</td>
        <td align='center'>Time</td>
        <td align='center'>Paper</td>
        <td align='center'>Code</td>
    </tr>
    <tr>
        <td align='center'>SayCan</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>04/2022</td>
        <td align='center'><a href="https://arxiv.org/pdf/2204.01691">Paper</a></td>
        <td align='center'><a href="https://say-can.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Social Simulacra</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>08/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.04024">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>TE</td>
        <td align='center'>Psychology </td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>08/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.10264">Paper</a></td>
        <td align='center'><a href="https://github.com/gatiaher/using-large-language-models-to-replicate-human-subject-studies">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Out of One</td>
        <td align='center'>Political Science and Economy</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>09/2022</td>
        <td align='center'><a href="https://arxiv.org/pdf/2209.06899">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>LangChain</td>
        <td align='center'>Psychology </td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>10/2022</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/hwchase17/langchain">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Blind Judgement</td>
        <td align='center'>Jurisprudence</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>01/2023</td>
        <td align='center'><a href="https://arxiv.org/pdf/2301.05327.pdf">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Horton</td>
        <td align='center'>Political Science and Economy</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>01/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2301.07543">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>DECKARD</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>01/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2301.12050">Paper</a></td>
        <td align='center'><a href="https://github.com/DeckardAgent/deckard">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Planner-Actor-Reporter</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>02/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.00763">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Auto-GPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>03/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/Significant-Gravitas/Auto-GPT">Code</a></td>
    </tr>
    <tr>
        <td align='center'>BMTools</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>03/2023</td>
        <td align='center'><a href="https://arxiv.org/pdf/2304.08354.pdf">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/BMTools">Code</a></td>
    </tr>
    <tr>
        <td align='center'>BabyAGI</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>04/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="yoheinakajima/babyagi">Code</a></td>
    </tr>
    <tr>
        <td align='center'>REFINER</td>
        <td align='center'>Psychology</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.01904">Paper</a></td>
        <td align='center'><a href="https://github.com/debjitpaul/refiner">Code</a></td>
    </tr>      
    <tr>
        <td align='center'>AgentGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.01904">Paper</a></td>
        <td align='center'><a href="https://github.com/reworkd/AgentGPT">Code</a></td>
    </tr>      
    <tr>
        <td align='center'>Generative Agents</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.03442">Paper</a></td>
        <td align='center'><a href="https://github.com/joonspk-research/generative_agents">Code</a></td>
    </tr>    
    <tr>
        <td align='center'>AI-legion</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>04/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/eumemic/ai-legion">Code</a></td>
    </tr>    
    <tr>
        <td align='center'>LoopGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2303.01665">Paper</a></td>
        <td align='center'><a href="https://github.com/farizrahman4u/loopgpt">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>SCG</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/pdf/2304.07590">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>AGiXT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>04/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/Josh-XT/AGiXT">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>IGLU</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Civil Engineering</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.10750">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>IELLM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Aerospace Engineering</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.14354">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>GPT4IA</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Industrial Automation</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.14721">Paper</a></td>
        <td align='center'><a href="https://github.com/YuchenXia/GPT4IndustrialAutomation">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>Workgpt</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>05/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/team-openpm/workgpt">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>AgentVerse</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>05/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/OpenBMB/AgentVerse">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>GPT Researcher</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.01852">Paper</a></td>
        <td align='center'><a href="https://github.com/assafelovic/gpt-researcher">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>SmolModels</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>05/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/smol-ai/developer">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>SuperAGI</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>05/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/TransformerOptimus/SuperAGI">Code</a></td>
    </tr>   
    <tr>
        <td align='center'>VOYAGER</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16291">Paper</a></td>
        <td align='center'><a href="https://github.com/MineDojo/Voyager">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>LLM4RL</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>06/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.03604">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>GPT Engineer</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>06/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/AntonOsika/gpt-engineer">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>MiniAGI</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>06/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/muellerberndt/mini-agi">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>DemoGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents;<br>CS&SE</td>
        <td align='center'>06/2023</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/melih-unsal/DemoGPT">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>TaPA</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.01848">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>Math Agents</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Science Education</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/pdf/2307.02502">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>SocialAI School</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.07871">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>Unified Agent</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.09668">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>S3</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.14984">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>Dialogue Shaping</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/pdf/2307.15833.pdf">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>ToolLLM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.16789">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ToolBench">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>ChatMOF</td>
        <td align='center'>-</td>
        <td align='center'>Document and Data Management</td>
        <td align='center'>-</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/pdf/2308.01423">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>MetaGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.00352">Paper</a></td>
        <td align='center'><a href="https://github.com/geekan/MetaGPT">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>AutoGen</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>General Autonomous Agents</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.08155">Paper</a></td>
        <td align='center'><a href="https://microsoft.github.io/FLAML/docs/Use-Cases/Autogen/">Code</a></td>
    </tr> 
</table>

*This table only summarizes partial previous work. See section [More comprehensive Summarization](#more-comprehensive-summarization) for more papers.*

## Evaluation on LLM-based Autonomous Agent
<table>
    <tr>
        <td align='center'>Model</td>
        <td align='center'>Subjective </td>
        <td align='center'>Objective </td>
        <td align='center'>Benchmark</td>
        <td align='center'>Time</td>
        <td align='center'>Paper</td>
        <td align='center'>Code</td>
    </tr>
    <tr>
        <td align='center'>WebShop</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Isolated Reasoning;<br> Multi-task Evaluation </td>
        <td align='center'>&check;</td>
        <td align='center'>07/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2207.01206">Paper</a></td>
        <td align='center'><a href="https://github.com/princeton-nlp/webshop">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Social Simulacra</td>
        <td align='center'>Human Annotation</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>-</td>
        <td align='center'>08/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.04024">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>TE</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>-</td>
        <td align='center'>08/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.10264">Paper</a></td>
        <td align='center'><a href="https://github.com/GatiAher/UsingLarge-Language-Models-to-Replicate-Human-Subject-Studies">Code</a></td>
    </tr>
    <tr>
        <td align='center'>LIBRO</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing</td>
        <td align='center'>-</td>
        <td align='center'>09/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2209.11515">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ReAct</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>10/2022</td>
        <td align='center'><a href="https://arxiv.org/abs/2210.03629">Paper</a></td>
        <td align='center'><a href="https://github.com/ysymyth/ReAct">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Out of One, Many</td>
        <td align='center'>Turing Test</td>
        <td align='center'> Isolated Reasoning;<br> Multi-task Evaluation</td>
        <td align='center'>-</td>
        <td align='center'>02/2023</td>        
        <td align='center'><a href="https://arxiv.org/abs/2209.06899">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>DEPS</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>02/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.01560">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Jalil et al.</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing</td>
        <td align='center'>-</td>
        <td align='center'>02/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.03287">Paper</a></td>
        <td align='center'><a href="https://github.com/sajedjalil/ChatGPT-Software-Testing-Stud">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Reflexion</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning</td>
        <td align='center'>-</td>
        <td align='center'>03/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2303.11366">Paper</a></td>
        <td align='center'><a href="https://github.com/noahshinn024/reflexion">Code</a></td>
    </tr>
    <tr>
        <td align='center'>IGLU</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.10750">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>LLM+P</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning</td>
        <td align='center'>-</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.11477">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Generative Agents</td>
        <td align='center'> Human Annoation;<br>Turing Test</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.03442">Paper</a></td>
        <td align='center'><a href="https://github.com/joonspk-research/generative_agents">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ToolLLM</td>
        <td align='center'>Human Annoation</td>
        <td align='center'>Multi-task Evalution</td>
        <td align='center'>&check;</td>
        <td align='center'>04/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.16789">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ToolBench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>GITM</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.17144">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenGVLab/GITM">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Two-Failures</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>-</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.14279">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Voyager</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16291">Paper</a></td>
        <td align='center'><a href="https://github.com/MineDojo/Voyager">Code</a></td>
    </tr>
    <tr>
        <td align='center'>SocKET</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning;<br> Social Evaluation;<br>Multi-task Evaluation </td>
        <td align='center'>&check;</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.14938">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Mobile-Env</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Isolated Reasoning;<br> Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.08144">Paper</a></td>
        <td align='center'><a href="https://github.com/X-LANCE/Mobile-Env">Code</a></td>
    </tr>
    <tr>
        <td align='center'>clembench</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>05/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.13455">Paper</a></td>
        <td align='center'><a href="https://github.com/clp-research/clembench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Dialop</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'>06/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.20076">Paper</a></td>
        <td align='center'><a href="https://github.com/jlin816/dialop">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ChatDB</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning</td>
        <td align='center'>-</td>
        <td align='center'>06/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.03901">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Feldt et al.</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing</td>
        <td align='center'>-</td>
        <td align='center'>06/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.05152">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>CO-LLM</td>
        <td align='center'>Human Annoation</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>-</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.02485">Paper</a></td>
        <td align='center'><a href="https://vis-www.cs.umass.edu/Co-LLM-Agents/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Tachikuma</td>
        <td align='center'>Human Annoation</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.12573">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChatDev</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning</td>
        <td align='center'>-</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.07924">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>WebArena</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'>07/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.13854">Paper</a></td>
        <td align='center'><a href="https://github.com/web-arena-x/webarena">Code</a></td>
    </tr>
    <tr>
        <td align='center'>AgentSims</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>-</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.04026">Paper</a></td>
        <td align='center'><a href="https://github.com/py499372727/AgentSims">Code</a></td>
    </tr>
    <tr>
        <td align='center'>AgentBench</td>
        <td align='center'>-</td>
        <td align='center'>Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.03688">Paper</a></td>
        <td align='center'><a href="https://github.com/thudm/agentbench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>BOLAA</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br>Multi-task Evaluation;<br>Software Testing</td>
        <td align='center'>&check;</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.05960">Paper</a></td>
        <td align='center'><a href="https://github.com/salesforce/BOLAA">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Gentopia</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning;<br> Multi-task Evaluation </td>
        <td align='center'>&check;</td>
        <td align='center'>08/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.04030">Paper</a></td>
        <td align='center'><a href="https://github.com/Gentopia-AI/Gentopia">Code</a></td>
    </tr>
</table>

*This table only summarizes partial previous work. See section [More comprehensive Summarization](#more-comprehensive-summarization) for more papers.*

<hr>

## More Comprehensive Summarization

We are maintaining an [interactive table](https://abyssinian-molybdenum-f76.notion.site/237e9f7515d543c0922c74f4c3012a77?v=0a309e53d6454afcbe7a5a7e169be0f9&pvs=4) that contains more comprehensive papers related to LLM-based Agents. This table includes details such as tags, authors, publication date, and more, allowing you to sort, filter, and find the papers of interest to you.
![Complete Table](assets/table.png)

## Maintainers
- Lei Wang@[Paitesanshi](https://github.com/Paitesanshi)
- Chen Ma@[Uily](https://github.com/Yilu114)
- Xueyang Feng@[XueyangFeng](https://github.com/XueyangFeng)


## Citation
If you find this survey useful, please cite our paper:
```
@misc{wang2023survey,
      title={A Survey on Large Language Model based Autonomous Agents}, 
      author={Lei Wang and Chen Ma and Xueyang Feng and Zeyu Zhang and Hao Yang and Jingsen Zhang and Zhiyuan Chen and Jiakai Tang and Xu Chen and Yankai Lin and Wayne Xin Zhao and Zhewei Wei and Ji-Rong Wen},
      year={2023},
      eprint={2308.11432},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
```
## How to Contribute
We warmly welcome contributions to this survey and interactive table. If you have a paper or know of relevant research that should be included, please contribute through pull requests, issues, email, or other methods.

## Acknowledgement
We thank the following people for their valuable suggestions and contributions to this survey:
- Yifan Song[@Yifan-Song793](https://github.com/Yifan-Song793)
- Qichen Zhao[@Andrewzh112](https://github.com/Andrewzh112)
- Ikko E. Ashimine[@eltociear](https://github.com/eltociear)


## Contact Us
If you have any questions or suggestions, please contact us via:
- Email: wanglei154@ruc.edu.cn


