# Hopfield Network for Image Recovery  

## Overview  
This project explores the implementation of a Hopfield network with Hebbian learning to recover 16×16 pixel images after corruption. The network is tested on a set of 25 patterns, with experiments conducted using both synchronous and asynchronous updates.  

## Features  
- Implements a Hopfield neural network with Hebbian learning.  
- Supports storage and recall of 16×16 binary images.  
- Corruption methods:  
  - Bit-flipping corruption.  
  - Box-filter corruption (10×10 pixel masking).  
- Comparison of synchronous and asynchronous update methods.  
- Analysis of convergence success rates under different probabilities of corruption.  

## Dataset  
- 25 hand-drawn 16×16 pixel images converted to `.pbm` format.  
- Experiments show that storing and recalling three images at once provides the best convergence performance.  

## Results  
- With a large number of stored patterns (25), the network fails to converge correctly.  
- A subset of 3–4 images shows successful convergence when corruption probabilities are adjusted.  
- The number of update steps required for convergence remains consistently around three.  

