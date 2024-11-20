<h1 align="center">Boltz-1:

Democratizing Biomolecular Interaction Modeling
</h1>

![](docs/boltz1_pred_figure.png)

Boltz-1 is an open-source model which predicts the 3D structure of proteins, rna, dna and small molecules; it handles modified residues, covalent ligands and glycans, as well as condition the generation on pocket residues. 

For more information about the model, see our [technical report](https://gcorso.github.io/assets/boltz1.pdf).

## Installation
Install boltz with PyPI (recommended):

```
pip install boltz
```

or directly from GitHub for daily updates:

```
git clone https://github.com/jwohlwend/boltz.git
cd boltz; pip install -e .
```
> Note: we recommend installing boltz in a fresh python environment

## Inference

You can run inference using Boltz-1 with:

```
boltz predict input_path
```

Boltz currently accepts three input formats:

1. Fasta file, for most use cases

2. A comprehensive YAML schema, for more complex use cases

3. A directory containing files of the above formats, for batched processing

To see all available options: `boltz predict --help` and for more informaton on these input formats, see our [prediction instructions](docs/prediction.md).

## Training

If you're interested in retraining the model, see our [training instructions](docs/training.md).

## Contributing

We welcome external contributions and are eager to engage with the community. Connect with us on our [Slack channel](https://boltz-community.slack.com/archives/C0818M6DWH2) to discuss advancements, share insights, and foster collaboration around Boltz-1.

## Coming very soon

- [x] Auto-generated MSAs using MMseqs2
- [x] More examples
- [ ] Support for custom paired MSA
- [ ] Confidence model checkpoint
- [ ] Pocket conditioning support
- [ ] Full data processing pipeline
- [ ] Colab notebook for inference
- [ ] Kernel integration

## License

Our model and code are released under MIT License, and can be freely used for both academic and commercial purposes.


## Cite

If you use this code or the models in your research, please cite the following papers:

```bibtex
@article {Wohlwend2024.11.19.624167,
	author = {Wohlwend, Jeremy and Corso, Gabriele and Passaro, Saro and Reveiz, Mateo and Leidal, Ken and Swiderski, Wojtek and Portnoi, Tally and Chinn, Itamar and Silterra, Jacob and Jaakkola, Tommi and Barzilay, Regina},
	title = {Boltz-1: Democratizing Biomolecular Interaction Modeling},
	elocation-id = {2024.11.19.624167},
	year = {2024},
	doi = {10.1101/2024.11.19.624167},
	publisher = {Cold Spring Harbor Laboratory},
	URL = {https://www.biorxiv.org/content/early/2024/11/20/2024.11.19.624167},
	eprint = {https://www.biorxiv.org/content/early/2024/11/20/2024.11.19.624167.full.pdf},
	journal = {bioRxiv}
}
```

```bibtex
@article{mirdita2022colabfold,
  title={ColabFold: making protein folding accessible to all},
  author={Mirdita, Milot and Sch{\"u}tze, Konstantin and Moriwaki, Yoshitaka and Heo, Lim and Ovchinnikov, Sergey and Steinegger, Martin},
  journal={Nature methods},
  volume={19},
  number={6},
  pages={679--682},
  year={2022},
  publisher={Nature Publishing Group US New York}
}
```