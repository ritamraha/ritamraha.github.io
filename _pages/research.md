---
title: "Research"
layout: default
sitemap: false
permalink: /research/
---

## Research

My research interest includes Verification of AI, Automata Theory, and Games. I am currently working on two aspects of theoretical foundations of formal verification techniques: i. Learning from data ii. Formal Verification of systems. More details about each of the aspects have been discussed below.

<div class="jumbotron">
<div class="row">
<div class="col-md-9 col-sm-12">
 <h4>Learning</h4>

 Towards the explanation and learning specifications of complex systems, we focus on logical models. In particular, it aims to learn formulas in temporal logic (e.g. Linear Temporal Logic, Signal Temporal Logic etc.). These logics can specify temporal specifications and hence have been a de facto standard in the field of formal verification and learning. Over the past few years, learning temporal logics has been identified as an important goal in the field of robotics, specification mining, and AI. Explanation in temporal logics is especially desirable as they are not only mathematically rigorous but also resemble natural language as argued in the literature.
 The fundamental problem is to build an explainable specification in the form of a temporal logic formula from a set of positive and negative execution traces of a system. We have developped algorithms for learning LTL specifications from labelled execution traces of the system which is given as an input. The work led to <a href="https://dblp.org/rec/journals/corr/abs-1909-07653">this paper</a>. We also developped a python based tool called <a href= "https://scarlet.labri.fr/">*SCARLET*</a> which generates LTL specifications from system traces.

</div>
</div>
</div>


<div class="jumbotron">
<div class="row">
<div class="col-md-9 col-sm-12">
<h4>Verification</h4>

The verification of complex systems comprises techniques for providing a formal proof on an abstract for- mal model of the system. There are many such classical mathematical models in the literature like finite state machines, Petri nets, vector addition systems etc. In the thesis, we consider One-Counter automata with parameters(POCA) as the abstract model. These are particularly useful for modelling the behaviour of pro- grams whose control flow is determined by counter variables. Execution of such programs can also be over- approximated by its control-flow graph (CFG), but it is prone to produce false negative results as the abstrac- tion is too coarse. A natural refinement can be obtained by using the POCA model we consider. POCA are ex- tension of finite state automata with a counter that can be updated or tested with constants or parameters in the transitions.
One of the main approaches of verification, that I worked on, is the parameter-synthesis problem that asks if there exists a valuation of the parameters such that all executions of a system satisfies some specification or not. For example, given a variable x and a critical section in a piece of code, we are interested in the question “is there a value of variable x for which the critical section can be avoided?”. We showed decidability results for the LTL parameter-synthesis problem for POCA in <a href="https://drops.dagstuhl.de/opus/volltexte/2022/15753/">this paper</a>. 

</div>
</div>
</div>
 

<div class="jumbotron">
<div class="row">
<div class="col-md-9 col-sm-12">
 <h4>Master's Thesis (Games)</h4>

<p>I have done my Master's thesis on <span style= "color:#F14E23"><b><i>Relaxed Energy Games</i></b></span> at <a href="https://www.irisa.fr/sumo/">SUMO team </a>, INRIA, Rennes under supervision of <a href="https://people.irisa.fr/Nicolas.Markey/">Nicolas Markey</a> and <a href="https://people.irisa.fr/Loic.Helouet/">Lo&iuml;c H&eacute;lou&euml;t</a>. My thesis led to <a href="https://dblp.org/rec/journals/corr/abs-1909-07653">this paper</a>.</p>
        
  <p> You can check my <b>thesis presentation</b> by clicking <a href="thesis/index.html" target="_blank">here</a> with the <b>thesis report</b> <a href="../papers/master_thesis.pdf" target="_blank">here</a> .</p>
  
  <i>Abstract:</i>
  <p> Energy reachability games are finite two player turn-based games played on weighted graphs. The objective of the game combines reachability objective(qualitative) with the (quantitative) requirement that the weights along a path must satisfy certain constraints (bounds). Besides having direct applications in reactive system synthesis with resource constraints, it is one of thesimplest models that combine quantitative and qualitative objectives.</p>

  <p> In this thesis, we first prove that under strict energy constraints (either only lower-bound constraint or interval constraint), those games are LOGSPACE-equivalent to energy games with the same energy constraints but without reachability objective (i.e., for infinite runs). We then consider two kinds of relaxations of the upper-bound constraints (while keeping the lower-bound constraint strict): in the first one, called weak upper bound, the upper bound is absorbing, in the sense that it allows receiving more energy when the upper bound is already reached, but the extra energy will not be stored; in the second one, we allow for temporary violations of the upper bound, imposing limits on the number or on the amount of violations. We prove that when considering weak upper bound, reachability objectives require memory, but can still be solved in polynomial-time for one-player arenas; we prove that they are in coNP in the two-player setting. Allowing for bounded violations makes the problem PSPACE-complete for one-player arenas and EXPTIME-complete for two players.
</p>

</div>
</div>
</div>
