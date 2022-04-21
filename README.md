# SpecialConceptBottleneck

This is a revised version of ConceptBottleneck experiment. Original Paper is [Concept Bottleneck Models](https://arxiv.org/abs/2007.04612)

to run on local machiene, need to change the address of picture in 
```angular2html
ConceptBottleneck/CUB/dataset.py
```

code to run the file on windows
* log_dir: anyfolder to save the log 
* data_dir: save the sorted data pickle file 
* the file address is the experiments in ConceptBottleneck
```shell
python D:\pycharmPool\SpecialConceptBottleneck\ConceptBottleneck\experiments.py cub Concept_XtoC --seed 1 -ckpt 1 -log_dir D:\pycharmPool\outputs\outputs -e 1000 -optimizer sgd -pretrained -use_aux -use_attr -weighted_loss multiple -data_dir D:\pycharmPool\DataFile\class_attr_data_10 -n_attributes 112 -normalize_loss -b 64 -weight_decay 0.00004 -lr 0.01 -scheduler_step 1000 -bottleneck
```
