# The Method of Simulated Quantiles

This is a simple repo to implement the Method of Simulated Quantiles by Dominicy and Veredas in Python. 

I build [agent-based](https://en.wikipedia.org/wiki/Agent-based_model) simulation models in [economics](http://www2.econ.iastate.edu/tesfatsi/abmread.htm). 

These models traditionally have a few methodological difficulties:

1. agent behavior: rational expectations is often not possible, so behavior must come from somewhere, and
2. estimation is not straightforward.

Much of my research is devoted to addressing the first question with tools from dynamic optimization, reinforcement learning, and approximate dynamic programming. 

**This repo**, however, is devoted to addressing the second question: how to *estimate* agent-based models. 

I am increasingly convinced that simulation-based structural estimation techniques are the most appropriate to apply to agent-based models. (See this [excellent blog post](http://fxdiebold.blogspot.com/2013/07/more-on-strange-american-estimator-gmm.html) by Francis Diebold for a succinct outline of why I increasingly hold this view.)

This repo will implement and test a baseline implementation of a promising MSM estimator, the "method of simulated quantiles." I think this estimator is particularly attractive for agent-based modeling because ABMs often produce distributions of a wide range of state and choice variables as a natural outcome of their execution. Because emergent properties, skew distributions, and complex distributions are often observed in ABMs, the quantiles-based approach is particularly attractive. 

The rest of this repo contains notebooks and code files which implement one of the examples Dominicy and Veredas implement to illustrate their method. 

Finally, references: 

- [Dominicy and Veredas (2013), Method of Simulated Quantiles](http://www.sciencedirect.com/science/article/pii/S0304407612001947) at ScienceDirect
    - [SSRN WP version](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1561185&rec=1&srcabs=770785&alg=7&pos=8)
- [McCulloch (1986), Simple consistent estimators of stable distribution parameters](http://www.tandfonline.com/doi/abs/10.1080/03610918608812563) 
    - [Author's draft version](http://www.econ.ohio-state.edu/jhm/papers/stabparm.pdf)


