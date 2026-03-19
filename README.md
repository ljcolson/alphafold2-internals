# AlphaFold Internals: From MSA Signals to 3D Structure

## Overview
This project investigates how AlphaFold-like models transform evolutionary information from multiple sequence alignments (MSAs) into accurate 3D protein structures. Rather than treating the model as a black box, I use the OpenFold implementation to probe and analyze its internal representations.

## Key Goals
- Trace how MSA features propagate through the Evoformer (`m` and `z` representations)
- Connect statistical signals in MSAs (e.g., conservation, coevolution) to learned model representations
- Analyze how structural confidence metrics (pLDDT, PAE) emerge during inference
- Evaluate how MSA composition affects prediction accuracy and stability

## Approach
I built a lightweight, inspectable framework around OpenFold to extract intermediate tensors, run controlled experiments on MSA inputs, and visualize how structure predictions evolve across model components.

## Running
This notebook can be run on Google Colab (CPU runtime works)
