Hi, I'm Jake a software engineer and mathematician. 

<div style="height: 15px;"></div>

I recently solved a 50-year Erd&#337;s conjecture with Opus 4.8 by first establishing a density one normal order for [Erd&#337;s problem #685](https://www.erdosproblems.com/forum/thread/685),

<div align="center">
  <img width="700" alt="image" src="https://github.com/user-attachments/assets/797bad59-fbba-4840-850d-336a4b490f81" />
</div>

which enabled a three-argument [solution](https://www.researchgate.net/publication/409471385_Erdos_Problem_685_at_Density_One_An_Unconditional_Proof_of_the_Erdos-Gupta-Khare_Second-Moment_Conjecture) of the second moment.

researched the efficacy of computer vision for the ___UNKNOT RECOGNITION___ and ___KNOTTEDNESS___ problems, i.e. deciding whether a given knot diagram represents the unknot or a non-trivial knot.

To gather results, I built: [seeing-the-unknot](https://github.com/jakeweatherhead/seeing-the-unknot), a computer vision fine-tuning pipeline built using PyTorch and [GradCAM](https://github.com/jacobgil/pytorch-grad-cam) for explainability.

<div style="height: 15px;"></div>

<div align="center">
  <img width="1195" height="246" alt="image" src="https://github.com/user-attachments/assets/88f593e4-3402-460d-82be-f3434852b640" />
  <br />
  <sup>Saliency maps generated with GradCAM (https://github.com/jacobgil/pytorch-grad-cam).</sup>
</div>

<div style="height: 15px;"></div>

This led to my [thesis](https://github.com/jakeweatherhead/knot-theory-thesis), which to my knowledge, is the first academic contribution providing evidence of computer vision's ability to determine knot-triviality in knot diagrams.

<div style="height: 15px;"></div>

As we scaled to larger datasets of more complex knots, it was clear that the performance of [seeing-the-unknot](https://github.com/jakeweatherhead/seeing-the-unknot) was a major bottleneck for our continued research-velocity.

<div style="height: 15px;"></div>

So, as a fun exercise at the end of my degree, I investigated machine learning performance optimisation, learned about CUDA kernel fusion, and wrote a PyTorch C++ extension.

<div style="height: 15px;"></div>

My CUDA kernel would never challenge NVIDIA's CUTLASS, but determinstic dispatch via C++ did eliminate tail latencies in the convolutional weight gradient calculation. 

<div align="center">
  <img width="800" alt="image" src="https://github.com/user-attachments/assets/0036a528-f5c6-479b-9d82-2f2fd44fbfed"/>
</div>
