# Elevation of MLsec
Elevation of MLsec is an unofficial Machine Learning Security (MLsec) extension of Microsoft's Elevation of Privilege threat modeling card game. These playing cards portray risks associated with machine learning (ML) that have been identified by research groups. It is suitable to play this game with or without the original Elevation of Privilege deck depending on the nature of what you're threat modeling. The intention of these cards is primarily to improve the security *of* ML systems themselves, as opposed to using ML for security.

<img src="./game/cards-example.png" alt="Example of a few cards from the game Elevation of MLsec"/>

## Source material

This work is based mainly on Berryville Institute for Machine Learnings (BIML)’s architectural risk analysis for machine learning systems (BIML-78) and their LLM analysis (BIML-LLM24), found on [berryvilleiml.com](https://berryvilleiml.com). We have also added a few somewhat supplementary LLM specific threats from OWASP’s TOP 10 list for Large Language Model Applications found on [owasp.org](https://owasp.org/www-project-top-10-for-large-language-model-applications/).


For this game we have created a derivative of the BIML risk framework into a simpler framework which considers four things: Dataset risks, Input risks, Model risks and Output risks (DIMO). The things also include risks associated with the "interfaces" between them. Read more about this in [game-risk-framework.md](./game-risk-framework.md).

To anyone curious about how the risk frameworks are mapped to our cards and applied in this game, please check out [risk-frameworks.md](./ml-risk-frameworks/risk-frameworks.md) and [cards.yaml](./game/cards.yaml). Please note that this game is *not* a comprehensive representation of the risks framework. To get a more complete overview of the identified ML and LLM risks, we recommend bringing the frameworks along to threat modeling sessions. The source material for Elevation of MLsec can found in the [ml-risk-frameworks](./ml-risk-frameworks/) folder.

## Available versions

- There is a digital version published by TNG Technology Consulting GmbH, as a game mode in their Elevation of Privilege game: https://github.com/TNG/elevation-of-privilege. 
- The game can be purchased in print at Agile Stationery: https://agilestationery.com/collections/threat-modeling/products/elevation-of-machine-learning-security-card-game

## Audience

We hope that this game helps spread the message of the important work about securing AI, published by BIML and the OWASP foundation. 

The following roles may find use for these cards as a way to get started with security engineering in an organization that is employing machine learning in some way:
1) Security practitioners can use this game to perform relevant threat modeling coaching with ML engineering teams. 
2) ML practitioners and engineers may use this deck as part of their thread modeling process. 
3) Software professionals integrating their "traditional software system" with an ML component can use these cards to get familiar with potential risks that come from integrating the ML component.

## Resources
- [BIML Risk framework adjusted for the game](./game-risk-framework.md)
- [The deck](./game/elevation-of-MLsec-cards.pdf)
- [Lined deck for print/cut](./game/print-ready/elevation-of-MLsec-print-ready-lined.pdf)
- [How to play](./game/how-to-play.md)
- [Overview of card contents in cards.yaml](./game/cards.yaml)
- [Source materials: ML risk frameworks](./ml-risk-frameworks/risk-frameworks.md)

## Licenses

Card templates are inspired by the Elevation of Privilege card game ([https://www.microsoft.com/en-us/download/details.aspx?id=20303](https://www.microsoft.com/en-us/download/details.aspx?id=20303)), which is © 2010 Microsoft Corporation, licensed under the Creative Commons Attribution 3.0 United States license ([https://creativecommons.org/licenses/by/3.0/us/](https://creativecommons.org/licenses/by/3.0/us/)). The original work has been modified. 

Contents are based on Berryville Institute for Machine Learning (BIML) Architectural Risk Frameworks for Machine Learning and Large Language Models (BIML-78 and BIML-LLM24) which are published under a Creative Commons Attribution-Share Alike 3.0 License. We have also used the OWASP Top 10 for Large Language Model Applications, which is  published under Creative Commons Attribution-ShareAlike v4.0. Parts of the original work have been changed, and some descriptions are copied verbatim. We have added the original papers in the ML-risk-frameworks folder.

Elevation of MLSec is © 2024 Kantega AS. This work is licenced under the Creative Commons Attribution-ShareAlike 4.0 International license ([https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)).

## Working group
- Author: Elias Brattli Sørensen
- Designer: Jorun Kristin Bremseth

### Acknowledgements
We would like to thank Emil Jakobus Schroeder, Edvard Kristoffer Karlsen and August Heltne for QA and advice, and our employer Kantega AS for letting us produce this game.


