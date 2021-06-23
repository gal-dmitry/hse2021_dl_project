
# Deep Learning final project assignment

**Team: 13**

**Theme 3: "Neural Arithmetic Logic Units"**

## References

### Papers
- [NALU](https://arxiv.org/pdf/1808.00508.pdf)
- [NALU investigation](https://github.com/FrederikWarburg/latent_disagreement)
- [iNALU](https://arxiv.org/pdf/2003.07629v1.pdf)
- [NPU](https://arxiv.org/pdf/2006.01681.pdf)
- [NAU, NMU](https://openreview.net/pdf?id=H1gNOeHKPS)

### GitHub repositories
- [NALU](https://github.com/kevinzakka/NALU-pytorch)
- [NPU, NMU, iNALU, NALU (Julia)](https://github.com/nmheim/NeuralArithmetic.jl)

## Models:

Code: 
- [NAC](./models/nac.py)
- [Complex_NAC](./models/complex_nac.py)
- [NALU](./models/nalu.py)
- [NPU, NAU](./models/npu.py)


## Experiments

| ID | Description | Model | Layers | Arithmetic function | Link |
| :-: | :-: | :-- | :-: | :-- | :-: |
| 1 | Проверить, что значения обученных матриц W_hat, M_hat принадлежат {-1, 0, 1} | | | | [`Experiment_1.ipynb`](Experiment_1.ipynb) |
| 1.1 | | NAC&#160;(+,&#160;-) | 1 | x_1 + x_2 | |
| 1.2 | | NAC&#160;(+,&#160;-) | 1 | x_1 - x_2 | |
| 1.3 | | NAC&#160;(*,&#160;/) | 1 | x_1 * x_2 | |
| 1.4 | | NAC&#160;(*,&#160;/) | 1 | x_1 / x_2 | |
| | | | | |
| 2 | Проверить, что значения обученной матрицы G принадлежат {0, 1} | | | | [`Experiment_2.ipynb`](Experiment_2.ipynb) |
| 2.1 | | NALU | 1 | x_1 + x_2 | |
| 2.2 | | NALU | 1 | x_1 * x_2 | |
| | | | | |
| 3 | Сравнить качество различных моделей <br /> (4.1 Simple Function Learning Tasks)[https://papers.nips.cc/paper/2018/file/0e64a7b00c83e3d22ce6b3acf2c582b6-Paper.pdf] | | | | [`Experiment_3.ipynb`](Experiment_3.ipynb) |
| | | NALU <br /> NAC&#160;(+,&#160;-) <br /> NAC&#160;(*,&#160;/) <br /> NPU <br /> Others(?) <br />| 2 |  | |
| 4 | Сравнить качество различных моделей <br /> (4.2 Simple Arithmetic Task)[https://arxiv.org/pdf/2006.01681.pdf] | | | | `Experiment_4.ipynb` (TO DO) |
| | | NALU <br /> NAC&#160;(+,&#160;-) <br /> NAC&#160;(*,&#160;/) <br /> NPU <br /> Others(?) <br />| 2 |  | |


Wandb repositories of experiments:

- [Experiment_1](https://wandb.ai/galmitr/Experiment_1)
- [Experiment_2](https://wandb.ai/galmitr/Experiment_2)
- [Experiment_3_INTRO](https://wandb.ai/galmitr/INTERPOLATION)
- Experiment_3_EXTRO (TO DO)
- Experiment_4 (TO DO)


Report:

[Google Colab file: `Report.ipynb`](https://colab.research.google.com/drive/1icQ92gBv-kuD7pY39xzeKBe6cJx9pAyU?usp=sharing)