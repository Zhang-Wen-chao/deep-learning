# deep-learning
开始复现stable diffusion和dalle 2

   - [ ] vit，clip。对齐，位置，第一步。generation，dalle2：给定smiles，就可以当作图像的特征，但未必是真的图像特征。再decoder，autoregressve、diffusion。第二种做法就是stable diffussion。先做一个图像的特征，aotuencoder，给定condition生成一个图像的特征。反正第一步是对齐文本和图像的特征。给个graph生成图像，给个文本生成图像，可以都做。

```bash
conda env create -f environment.yml

conda env export > environment.yml

conda env export --name <environment_name> > environment.yml

```
