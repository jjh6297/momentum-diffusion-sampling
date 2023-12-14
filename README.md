# Momentum_Diffusion_Sampling

<!---Code for ["Rethinking Peculiar Images by Diffusion Models: Revealing Local Minima’s Role"]-->

## Updates


- 15/08/2023: Project page built


## Abstract

Recent significant advancements in diffusion models have revolutionized image generation, enabling the synthesis of highly realistic images with text-based guidance. These breakthroughs have paved the way for constructing datasets via generative artificial intelligence (AI), offering immense potential for various applications. However, two critical challenges hinder the widespread adoption of synthesized data: computational cost and the generation of peculiar images. While computational costs have improved through various approaches, the issue of peculiar image generation remains relatively unexplored. Existing solutions rely on heuristics, additional training, or AI-based post-processing to mitigate this problem. In this paper, we present a novel approach to address both issues simultaneously. We establish that both gradient descent and diffusion sampling are specific cases of the generalized expectation-maximization algorithm. We hypothesize and empirically demonstrate that peculiar image generation is akin to the local minima problem in traditional optimization. Inspired by optimization techniques, we apply naive momentum and positive-negative momentum to diffusion sampling. At last, we propose two novel metrics to evaluate the peculiarity. Experimental results show momentum effectively prevents peculiar image generation, yielding natural images without extra computation.



## requirements

Our implementation is based on "https://github.com/divamgupta/stable-diffusion-tensorflow".
Please download and install the baseline repository.


## Usage

you can generate images from a text prompt using:
```
python text2image_Momentum.py --prompt="An astronaut riding a horse"
```
#
