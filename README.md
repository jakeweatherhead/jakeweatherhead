I'm a software engineer in Pretoria, South Africa researching the efficacy of computer vision for the ___UNKNOT RECOGNITION___ and ___KNOTTEDNESS___ problems, i.e. deciding whether a given knot diagram represents the unknot or a non-trivial knot.

To gather results, I built: [seeing-the-unknot](https://github.com/jakeweatherhead/seeing-the-unknot), a computer vision fine-tuning pipeline built using PyTorch.

This led to my [thesis](https://github.com/jakeweatherhead/knot-theory-thesis), which to my knowledge, was the first academic contribution providing evidence of computer vision's ability to determine knot-triviality from knot diagrams.

As our investigations scaled to larger datasets of more complex knots (w.r.t. diagrammatic crossing count), it was clear that the performance of the [seeing-the-unknot](https://github.com/jakeweatherhead/seeing-the-unknot) fine-tuning pipeline was a bottleneck for our research-velocity going forward.

So, as fun exercise towards the end of my degree, I investigated potential remedies, learned about CUDA kernel fusion, and wrote a PyTorch C++ extension.

Performance did improve, but not for the reasons I expected. My kernel would never challenge NVidia's CUTLASS, but determinstic dispatch via C++ did eliminate significant tail latencies in the convolutional weight gradient calculation. 

<div align="center">
  <img src="https://github.com/user-attachments/assets/5c8d3a7e-b3c1-477f-b5de-35dfd80f6d20" alt="githubthreeknotnegative" width="600"/>
</div>

<br>
<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=python,cpp,linux" />
  </a>
</p>
