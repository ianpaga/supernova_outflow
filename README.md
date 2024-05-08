Supernova outflow model: subsonic & supersonic outflows 
====

This Mathematica notebook reproduces the results of the following paper https://arxiv.org/pdf/2009.10059

The goal is to solve the outflow equations which form a coupled system of differential equations:

<img width="439" alt="Screenshot 2024-05-07 at 19 01 02" src="https://github.com/ianpaga/supernova_outflow/assets/57350668/748d1bdd-5fc7-4155-a5d9-427975704554">

These expressions take into account the change in the effective number of relativistic degrees of freedom g_star, 
which occurs as the outflow cools through the temperature of the e+e- annihilation between the proton-neutron-star 
surface and the outer edges of the hot bubble. If one wants to neglect relativistic effects, the derivative of the logs is zero.

As the outflows accelerators to supersonic speeds and the sonic point (v = vs), being a mathematical singularity, 
require some care. Next, one can use this wind solution up to the location of the termination shock. 
At this point, the density and velocity jump and the change in velocity at the termination shock is given by the Rankine-Hugoniot jump condition:

<img width="513" alt="Screenshot 2024-05-07 at 19 21 42" src="https://github.com/ianpaga/supernova_outflow/assets/57350668/eb4a12af-9114-4281-84be-1cb91ab1b9c7">

where v1, T1, and S1 are the pre-shock quantities and therefore are taken from the wind solution at the location of the termination shock. 
 
In this Mathematica notebook, we show how to calculate the subsonic and supersonic solutions, and how to find the velocity at the termination shock. 
For more details, we refer the reader to Ref https://arxiv.org/pdf/2009.10059 and in particular Figs. 2 and 4 for a one-to-one comparison between 
my results and those reported in that paper.

Results from the notebook:

<img width="360" alt="plot2" src="https://github.com/ianpaga/supernova_outflow/assets/57350668/495b2acf-04c3-48fa-aa2b-e3560ce92382">
<img width="360" alt="plot1" src="https://github.com/ianpaga/supernova_outflow/assets/57350668/43656cc3-f7b0-4e07-b592-1ce860b70921">

## Requirements

- Mathematica 
