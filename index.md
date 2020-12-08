## Description

Database research is facing a reproducibility crisis, despite the encouragement by
multiple initiatives. The lack of open artifacts, most importantly data and source code,
obstructs the validation of existing research hindering our community’s progress. 
We aim to evaluate the status quo of reproducibility in data integration,
focusing on four data integration tasks: schema matching, schema mapping, entity matching 
and entity resolution. 

We investigated artifacts from 27 papers and measured their  reproducibility. 
Apart from a thorough study of the current situation, we introduce a reproducibility 
checklist for data integration, and a newly proposed metric for assessing a research
paper’s degree of reproducibility during the review process. This survey shows that
less than 10% of the papers can be fully reproduced and that there
are substantial differences in the degree of reproducibility among different data
integration tasks. Beside the checklist and the metric, we also propose 
actionable steps to move forward. 

## Authors 

<div> 
<figure class="item" style="vertical-align:top; display: inline-block; text-align:center; width:200px">
    <a href="https://andraionescu.github.io/" target="_blank">
        <img alt="Andra Ionescu" src="./assets/img/andra_ionescu.jpg" height="auto" width="80" style="border-radius:50%"/>
    </a>
    <figcaption class="caption" style="display:block">Andra Ionescu <br>TU Delft</figcaption>
</figure>

<figure class="item" style="vertical-align:top; display: inline-block; text-align:center; width:200px">
    <a href="http://mariosfragkoulis.gr/" target="_blank">
        <img alt="Marios Fragkoulis" src="./assets/img/marios_fragkoulis.jpg" height="auto" width="80" style="border-radius:50%"/>
    </a>
    <figcaption class="caption" style="display:block">Marios Fragkoulis <br> TU Delft</figcaption>
</figure>

<figure class="item" style="vertical-align:top; display: inline-block; text-align:center; width:200px">
    <a href="https://www.tudelft.nl/ewi/over-de-faculteit/afdelingen/software-technology/web-information-systems/people/christoph-lofi/" target="_blank">
        <img alt="Christoph Lofi" src="./assets/img/christoph_lofi.jpg" height="auto" width="80" style="border-radius:50%"/>
    </a>
    <figcaption class="caption" style="display:block">Christoph Lofi <br>TU Delft</figcaption>
</figure>

<figure class="item" style="vertical-align:top; display: inline-block; text-align:center; width:200px">
    <a href="http://asterios.katsifodimos.com/" target="_blank">
        <img alt="Asterios Katsifodimos" src="./assets/img/asterios_katsifodimos.jpg" height="auto" width="80" style="border-radius:50%"/>
    </a>
    <figcaption class="caption" style="display:block">Asterios Katsifodimos <br>TU Delft</figcaption>
</figure>
</div>

## Reproducibility checklist
The checklist is a projection of the minimum necessary to reproduce a paper in data
management. We use three categories (method, data, experiment) that were also used in 
other adjacent domains such as Artificial Intelligence and Machine Learning. 

### Method variables 
The variables from this category help a researcher understand the problem solved, 
the goal of the proposed method, and the methodology to achieve it.

- [ ] Problem = The problem the research aims to solve is specified
- [ ] Objective = The goal of the research is indicated 
- [ ] Contribution/Research Questions = The goal of the research is indicated  
- [ ] Research Methodology = The  research  methodology  is  described  (the  means  on  how  to achieve the objective)  
- [ ] Pseudo-code = The pseudo-code exists in the paper (does not apply if the sourcecode is provided)  
- [ ] Parameters/Threshold description = The parameters used by the algorithms are described 

### Data variables
The role of the Data type variables is to describe the datasets used in a paper.

- [ ] Experiment Data = At least one open-source available dataset is present or means on how to generate the data are provided
- [ ] Ground Truth/Gold Standard = The ground truth is given or means on how to create it are indicated 
- [ ] Data Version(\*) = The dataset version is provided 
- [ ] Parameters to create/export data(\*) = The parameters to create/export the data are specified 

### Experiment variables
The  variables  from  the Experiment type describe how experiments are conducted, 
including information about the environment, and the source code.

- [ ] Source Code = The code is open-sourced and available
- [ ] External Source Code(\*) = The source code is not mentioned in the paper, but external re-sources are available upon search  
- [ ] Experiment Source Code = The  URL  to  the  open-source  experiment  code  is  given  or  the experimental pipeline exists in the source code) 
- [ ] Experiment Setup = Details about how the experiments were conducted such as testing specific  parts  of  the  solution,  using  a  certain  configuration,  the metrics used are indicated  
- [ ] Parameters/Thresholds Value(\*) = The values for the parameters are provided  
- [ ] Hardware Specification = The description of the machine(s) used for experiments is present  
- [ ] Runtime = The indication of how long does the algorithm run on the specified hardware  

## Metric
The metric proposed is purely an indication of the amount of details available and missing.
Therefore, for each category, compute the percentage of the variables with _True_ and _False_
values. 

## How to move forward
1. Create workshops and challenges about reproducibility. 
2. Collaborate with open source software. 
3. Invest effort in hosting the data and artifacts in long-term storage as we do for the papers.
4. **Help change the culture!** Use the checklist to publicly show the reproducibility level
of your paper, encourage PhD students to work on making their artifacts openly available 
   and reproducible. 