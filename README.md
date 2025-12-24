# Agent-coalition-min-conflict
Project Overview The Iterated Symmetric Distributed Min-Conflict Heuristic (ISD-MCH) is a decentralized coordination algorithm designed for resource-constrained IoT devices and V2X (Vehicle-to-Everything) systems. It solves the Maximum Clique Completion Problem (MCCP) to form conflict-free agent coalitions in real-time.

Key Features



Decentralized Execution: 


No central controller; every agent runs the heuristic locally


.Bitwise Acceleration: Utilizes Non-Adjacency Masks (NAM) for $O(1)$ conflict detection.


Stagnation Recovery: Implements a stochastic restart mechanism to escape local maxima in structured graphs (e.g., Keller 3benchmarks).


V2X Optimized: Optimized for low-latency performance (average < 70ms), fitting within the 100ms V2X heartbeat.


Repository Structure/src: Python implementation of the ISD-MCH algorithm.


data: Pre-calculated bitwise adjacency data for DIMACS Keller-3  benchmarks.


Citation


If you use this code or the pre-calculated datasets in your research, please cite our paper:



@article{bouneb2025isdmch,
  title={Beyond Exhaustive Search: A Fast Min-Conflict
Heuristic for Symmetric Group Coalition
Formation in Distributed IoT Environments},
  author={Zine El Abidine Bouneb},
  journal={uknown},
  year={2025}
}
