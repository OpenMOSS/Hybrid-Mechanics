# Mechanics of Long-Context Hybrid Models

Part 1.1: [From Hybrid Attention to Hybrid Position](https://github.com/OpenMOSS/Hybrid-Mechanics/blob/main/part1_1-hybrid_position.pdf) 

1. **From Hybrid Attention to Hybrid Position**. Hybrid models improve long-context performance and length extrapolation through hybrid position, combining NoPE with other position biases. 
2. **Seesaw Effect in Context Extension of SWA Hybrid**. The advantage of SWA-NoPE hybrids over LA-NoPE hybrids in long-context performance is reversed after long-context pretraining, especially for layer-wise hybrids, due to their **Short-Context Learning Trap in Context Extension**.
3. **No Free Lunch Effect in Length Extrapolation of LA Hybrid**. LA-NoPE hybrids are weaker than SWA-NoPE hybrids in extrapolation, but stronger within the training context.
4. **Tidal Effect in Collaboration of Hybrid Position**. Effective collaboration of hybrid position relies on a minority of high-hit-rate NoPE attention with coarse aggregation and a majority of low-entropy position-biased attention (i.e., RoPE attention and gated linear attention) for noise reduction.
5. **Short-Window Weariness and Long-Window Laziness of SWA Hybrid**. In length extrapolation, SWA hybrids with short window size perform better, but in context extension, SWA hybrids with sliding window extended to a larger size overcome the short-context trap better.
6. **Matthew Effect in Length Extrapolation of Hybrid Position**. Effective extrapolation of hybrid models requires SWA in position-biased attention and enhanced aggregation in NoPE attention.