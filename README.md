# hca
Holonic Cellular Automata (HCA)
================================

Project Description
--------------------

HCA is a multi-level feedback control simulator based on cellular automata (CA).

HCA organises CA into several levels, which interact via: 
i) aggregate state information (bottom-up / micro-macro); and 
ii) adaptation control signals (top-down / macro-micro). 

CA at different levels execute different rule sets, at different paces. Each CA at a lower level Lk is mapped to a single cell of a CA at a higher level Lk+1. The entire state of a lower CA is aggregated (based on the percentage of its live cells relative to a threshold) and used to set the state of the corresponding cell in a higher CA (live or dead). Conversely, the state of each cell in a higher CA controls the rule adaptation of the corresponding lower CA (live/dead state triggers expansive/regressive rules). 
These interactions are replicated between successive levels, until reaching the topmost level which only executes static rules. 
CA execute in parallel, with aggregate states and adaptation control travelling bottom-up and top-down through the HCA levels.

Project Organisation
---------------------

The project is organised as follows:

> _data_ folder: raw data, graphs and analysis of selected experiments / simulations; please have a look at the README files;

> _videos_ folder: videos illustrating selected HCA simulations;

Please also see the project's _wiki_ for furhter documentation.
