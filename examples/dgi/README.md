Deep Graph Infomax (DGI)
========================

- Paper link: [https://arxiv.org/abs/1809.10341](https://arxiv.org/abs/1809.10341)
- Author's code repo (in Pytorch):
  [https://github.com/PetarV-/DGI](https://github.com/PetarV-/DGI)


How to run
----------

Run with following:

```bash
python dgi_trainer.py --dataset=cora --hidden_dim=512 --lr=0.0005 --n_epoch=300
```

```bash
python dgi_trainer.py --dataset=citeseer --hidden_dim=512 --lr=0.0001 --n_epoch=500
```

```bash
python dgi_trainer.py --dataset=pubmed --hidden_dim=256 --lr=0.001 --n_epoch=500
```

Results
-------


|      Dataset      | Cora | Citeseer | Pubmed |
| :---------------: | :--: | :------: | :----: |
|   Author's Code   | 82.3 |   71.8   |  76.8  |
|     GammaGL(tf)   | 81.6 |   70.5   |  78.85 |
|     GammaGL(th)   | --.- |   --.-   |  --.-  |
|     GammaGL(pd)   | --.- |   --.-   |  --.-  |
|     GammaGL(ms)   | --.- |   --.-   |  --.-  |
|        DGL        | 81.6 |   69.4   |  76.1  |
