Hi, I'm Jake a software engineer and discrete mathematician living in Pretoria, South Africa. 

<div style="height: 15px;"></div>

I recently solved a 50-year Erd&#337;s conjecture with Opus 4.8 and GPT 5.6 Sol,

<div align="center">
  <img width="1068" height="299" alt="image" src="https://github.com/user-attachments/assets/b8d1fb64-5fc2-4def-a145-b6b15248cb3f" />
  <br />
  <sup>P. Erd&#337;s, H. Gupta, S. P. Khare,
  On the number of distinct prime divisors of binomial coefficients,
  Utilitas Math. 10 (1976), See https://users.renyi.hu/~p_erdos/1976-29.pdf</sup>
</div>

Establishing a density one normal order for Erd&#337;s problem [#685](https://www.erdosproblems.com/forum/thread/685) enabled a three-argument [solution](https://www.researchgate.net/publication/409471385_Erdos_Problem_685_at_Density_One_An_Unconditional_Proof_of_the_Erdos-Gupta-Khare_Second-Moment_Conjecture) of the second moment:

1. a Turán-Kubilius mean-square method for slowly varying subpolynomial $k$.
2. a reduction to smooth numbers in short intervals when $k$ exceeds the square root of $n$.
3. a finite-histogram argument that reconstructs the additive function $\omega_{\gt k}$ from finitely many multiplicative functions by Vandermonde inversion when $k$ does not exceed the square root of $n$.

Proving this conjecture taught me invaluable lessons about how to get the best out of AI to solve otherwise intractable problems.

---

For my undergraduate thesis, I researched the efficacy of computer vision for the $\mathrm{Unknot\\,Recognition}$ and $\mathrm{Knottedness}$ problems, i.e. deciding whether a given knot diagram represents the unknot or a non-trivial knot.

To train models, I built [seeing-the-unknot](https://github.com/jakeweatherhead/seeing-the-unknot), a computer vision fine-tuning pipeline built using [PyTorch](https://github.com/pytorch/pytorch) and [GradCAM](https://github.com/jacobgil/pytorch-grad-cam).

<div style="height: 15px;"></div>

<div align="center">
  <img width="1195" height="246" alt="image" src="https://github.com/user-attachments/assets/88f593e4-3402-460d-82be-f3434852b640" />
  <br />
  <sup>Saliency maps generated with GradCAM (https://github.com/jacobgil/pytorch-grad-cam).</sup>
</div>

<div style="height: 15px;"></div>

This led to my [thesis](https://github.com/jakeweatherhead/knot-theory-thesis), which shows how we achieved >98% accuracy on a dataset of over half a million knot diagrams for both the CNN and ViT which, to my knowledge, is the world's first academic contribution providing evidence of computer vision's ability to solve the _unknot recognition_ problem.

<div style="height: 15px;"></div>
