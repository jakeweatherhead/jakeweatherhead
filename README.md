Hi, I'm Jake a software engineer and mathematician. 

<div style="height: 15px;"></div>

I recently researched the efficacy of computer vision for the ___UNKNOT RECOGNITION___ and ___KNOTTEDNESS___ problems, i.e. deciding whether a given knot diagram represents the unknot or a non-trivial knot.

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
