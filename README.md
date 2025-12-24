# Agent-coalition-min-conflict
Project Overview The Iterated Symmetric Distributed Min-Conflict Heuristic (ISD-MCH) is a decentralized coordination algorithm designed for resource-constrained IoT devices and V2X (Vehicle-to-Everything) systems. It solves the Maximum Clique Completion Problem (MCCP) to form conflict-free agent coalitions in real-time.

Key FeaturesDecentralized Execution: No central controller; every agent runs the heuristic locally.Bitwise Acceleration: Utilizes Non-Adjacency Masks (NAM) for $O(1)$ conflict detection.Stagnation Recovery: Implements a stochastic restart mechanism to escape local maxima in structured graphs (e.g., Keller benchmarks).V2X Optimized: Optimized for low-latency performance (average < 70ms), fitting within the 100ms V2X heartbeat.Repository Structure/src: C/C++ implementation of the ISD-MCH algorithm./data: Pre-calculated bitwise adjacency data for DIMACS Keller-5 and Keller-6 benchmarks.clique_validation_report_d5.txt: Full 5D coordinate decoding and adjacency lists for the size-28 clique validation.Reproducing ResultsTo reproduce the experimental results reported in the paper:Clone the repository.Compile the source using gcc or clang (optimization flag -O3 recommended).Run the executable against the provided Keller adjacency matrices in the /data folder.CitationIf you use this code or the pre-calculated datasets in your research, please cite our paper:Code snippet@article{bouneb2025isdmch,
  title={Symmetric Distributed Min-Conflict Heuristic for Autonomous Group Formation in V2X Environments},
  author={Zine El Abidine Bouneb},
  journal={uknown},
  year={2025}
}
