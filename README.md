# stroop model, for neu/psy 330 spring 2019 

this repo replicates 
<a href="https://www.ncbi.nlm.nih.gov/pubmed/2200075">cohen et al (1990)</a>
w/ psyneulink composition (version==0.5.2.1)

### doc 

- `stroop_model.py`: the definition of the stroop model
- `stroop_stimulus.py`: the definition of the stroop task
- `run_exp_stroop.py`: run the standard stroop experiment
- `run_exp_soa.py`: run SOA experiment
- `analyze_soa.py`: analyze and plot the data generated by `run_exp_soa.py`
- `stroop-feedforward.ipynb` and `stroop-linear.ipynb`: two simplifications of the full stroop model, for teaching purpose


### the full model

here's the architecture... 

<img src="https://github.com/qihongl/stroop-pnlcomp/blob/master/imgs/STROOP-model.png" alt="model" height=300px>

### results

here's the main result, meant to qualitatively replicate fig 5 from cohen et al (1990). so in general, color naming is slower than word reading; color naming *red green* as "red" is much slower than word reading *red green* as "green", where *red green* = the word green painted in red. 

<img src="https://github.com/qihongl/stroop-pnlcomp/blob/master/imgs/stroop_0.2.png" alt="rt" height=350px>


here's another way to plot the data. these are kernel density estimates of the reaction time distributions.  

<img src="https://github.com/qihongl/stroop-pnlcomp/blob/master/imgs/rt_kde.png" alt="rt kde" height=450px>


and here's the SOA effect:  

<img src="https://github.com/qihongl/stroop-pnlcomp/blob/master/imgs/soa.png" alt="soa" height=300px>



References: 

[1] Cohen, J. D., Dunbar, K., & McClelland, J. L. (1990). On the control of automatic processes: a parallel distributed processing account of the Stroop effect. Psychological Review, 97(3), 332–361. Retrieved from https://www.ncbi.nlm.nih.gov/pubmed/2200075

[2] the code is based on all stroop model scripts I can find from psyneulink example scripts 
<a href="https://github.com/PrincetonUniversity/PsyNeuLink/tree/master/Scripts">here</a>, 
and most importantly,
<a href="https://github.com/PrincetonUniversity/PsyNeuLink/blob/master/Scripts/Examples/Stroop%20Basic.py">this</a> 
and 
<a href="https://github.com/PrincetonUniversity/PsyNeuLink/blob/master/Scripts/Laura%20Stroop.py">this</a>
