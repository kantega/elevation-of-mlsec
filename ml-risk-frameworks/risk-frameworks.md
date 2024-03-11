# Risk frameworks
The following risk frameworks are used for source material:

- BIML's Architectural Risk Analysis of Machine Learning Systems (BIML_78): https://berryvilleiml.com/results/ara.pdf
- BIML's Architectural Risk Analysis of Large Language Models (BIML_LLM_24): https://berryvilleiml.com/results/BIML-LLM24.pdf
- The OWASP Top 10 Risks for Large Language Model Applications (OWASP_LLM): https://owasp.org/www-project-top-10-for-large-language-model-applications/

Attached in this folder are the pdf sources of this work from the time of publication. As they are licensed under Creative Commons, these are rightfully redistributed in this repository. 
The BIML papers (and other works) may be found at [berryvilleiml.com](https://berryvilleiml.com/). The OWASP LLM Top 10 paper (and later updates) may be found at [owasp.org](https://owasp.org).

## Mapping from BIML
For anyone curious, the following describes our mapping from the main source of this work, the architectural risk analysis for machine learning systems (refered to as BIML-78). This might give you an idea of how the risk framework is applied in this card game. Please note that this game is in no way a comprehensive representation or application of the above risk frameworks. We have hand-picked the risks from the BIML risk analysis that we felt fit best in context of this game, and we have also pruned several overlaps between components (for example, looping is described in both the input and output components of the BIML framework).


<img src="./biml-78-framework.png" alt="BIML Risk Framework for a Generic Machine Learning process" />

**Figure 1:** The BIML Risk Framework for a Generic Machine Learning process. Source: https://berryvilleiml.com/interactive/


The mapping from BIML to our card suits goes as follows:

| BIML component (including LLM risks) | Elevation of MLsec suits                                 |
|--------------------------------------|----------------------------------------------------------|
| 1. Raw data in the world             | Input risk: 6<br>Dataset risk: 2, 3, 10, Q                |
| 2. Dataset assembly                  | Dataset risk: 4, 5, 6, 7                                |
| 3. Datasets                          | Dataset risk: 9, Q                                      |
| 4. Learning algorithm                | Model risk: 3, 4, 5, 9                                  |
| 5. Evaluation                        | Model risk: 2, 6<br>Dataset risk: 8                       |
| 6. Inputs                            | Input risk: 3, 4, 5, 9, 10, J, Q, K                     |
| 7. Model                             | Model risk: 10, J, Q, K                                 |
| 8. Inference algorithm               | Model risk: 7, 8<br>Input risk: 2, 8<br>Output risk: 8      |
| 9. Outputs                           | Output risk: 5, 6, 7, 9, K                              |
| 10. System                           | Input risk: 7<br>Output risk: 2, 3, J, Q<br>Dataset risk: J |


This is also transparent in [cards.yaml](../cards.yaml), as every card references its origin identifier from the source material.

### Introducing the DIMO framework in Elevation of MLsec
In this customized and simplified version of the BIML risk framework, we collect all the 9 components of the BIML risk framework into four categories, which form our four card suits. The four things (3. Datasets, 6. Inputs, 7. Model, 9. Outputs) lie exclusively within their suit, while the interfaces (1. Raw data in the world, 2. Dataset assembly, 4. Learning algorithm, 5. Evaluation, 8. Inference algorithms) and the system as a whole may appear in several suits. This forms our framework of Dataset risk, Input risk, Model risk and Output risk (DIMO), which you can see visualized in Figure 2. Read more about this in [dimo-framework.md](../dimo-framework.md).


<img src="./DIMO-eoml.png" alt="The DIMO model presented in Elevation of Mlsec" />

**Figure 2** The DIMO framework in Elevation of MLsec, as a simplified version of the BIML risk framework.



## Mapping from OWASP

Risks from OWASP have been hand-picked to get something supplementary that hasn't been explicitly formulated by our main source, BIML. We have currently only picked two threats from the OWASP LLM top 10:
- OWASP LLM08 (Excessive agency) in Output risk 10.
- OWASP LLM09 (Overreliance) in Output risk 4.

We find that the rest of the LLM risks described by OWASP are sufficiently covered by our main source in BIML's LLM analysis.

## Backreferences in the game

We have made sure to backreference every card's origin back to the source material, so it's easy to expand upon a certain risk described only briefly in a card by using the source material in a thread modelings session. The cards are referencing specifically to the identifiers from the risks they originate. We have slightly modified the identifiers to specify which framework they originate from. 
- Risks originating from BIML’s ML risk analysis for ML are tagged without any prefix: \[\<component label\>:\<risk number\>:\<descriptor>\]. 
- Risks originating from the BIML Architectural Risk Analysis of LLMs are tagged with an LLM prefix \[LLM:\<component label\>:\<risk number\>:\<descriptor\>\]. 
- Risks from OWASP are tagged with \[OWASP-\<project\>-\<number\>\], so for LLMs it’s \[OWASP-LLM-\<number\>\]. 
