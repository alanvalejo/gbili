## RGCLI

**About**

This is an alternative Python implementation of graph construction method RGCLI (Robust Graph that Considers Labeled Instances), published by Berton and Lopes (2016) [1]. The implementation is based on Kd-tree and Multi-threading and is faster than the original described in the paper, specially for large data sets.

**Usage**

> RGCLI execution

    python rgcli.py -f input/dataset.dat -l input/dataset.labels -1 20 -2 2

> Input: any numerical dataset with any delimiter for attributes

> Output: a weighted undirected graph in the format: filename + '-gbili.ncol'

**Parameters**

| Option					| Domain					| Description															|
|:------------------------- |:------------------------- |:--------------------------------------------------------------------- |
| -f, --filename			| string [FILE]				| Dataset as input file													|
| -o, --output				| string [FILE]				| Output file default .ncol list										|
| -l, --label				| string [FILE]				| List of labels points used to construct RGCLI 						|
| -1, --ke					| [1,n] Integer interval	| ke for KNN															|
| -2, --ki					| [1,n] Integer interval	| ki for RGCLI															|
| -t, --threads				| [0,n] Integer interval	| Number of  threads													|
| -e, --format				| ['ncol', 'pajek']			| Format output file													|
| -c, --skip_last_column	| [0,n] Integer interval	| Skip the last column													|

**References**

> [1] Berton, Lilian; Faleiros, T.; Valejo, A.; Valverde-Rebaza, J.; and Lopes, A. A.: RGCLI: Robust Graph that Considers Labeled Instances for Semi-Supervised Learning. Neurocomputing, (2016)

~~~~~{.bib}
@article{Berton_2016,
    author={Lilian Berton and Thiago de Paulo Faleiros and Alan Valejo and Jorge Valverde-Rebaza and Alneu de Andrade Lopes},
    title={RGCLI: Robust Graph that Considers Labeled Instances for Semi-Supervised Learning},
	journal={Neurocomputing},
    year={2016}
}
~~~~~
