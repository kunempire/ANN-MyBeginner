Dive into the respective code files for more details.

CNN is waiting to fill (as if).

## Structure

For the model paramter files too large to store, the files in related directories are empty for referrence.

```bash
.
├── data # dataset
│   └── train_dev_test.tar
├── helper # process tools
│   ├── get_data_and_model.sh
│   ├── mosedecoder # model evaluation tool
│   ├── preprocess.sh # preprocess dataset
│   ├── transformer.base.yaml # model arguments
│   └── utils.py # divide Chinese words with jieba
├── model # model paramter files
│   ├── cnn
│       └── wait_fill
│   └── transformer
│       └── step_final
│           ├── transformer.pdopt
│           └── transformer.pdparams
├── trained_models # pretrained models
│   ├── CWMT2021_step_345000.tar.gz
│   └── CWMT2021_step_345000
│       ├── vocab.ch.src # Chinese vocabulary
│       ├── vocab.en.tgt # English vocabulary
│       ├── transformer.pdopt
│       └── transformer.pdparams
├── transformer.ipynb # transformer code
├── cnn.ipynb # cnn code
└── visualdl # visual logs
    ├── transformer
    │   └── transformer.log
    └── cnn
        └── wait_fill

```

## Attention

Model evaluation tool `mosedecoder.tar.gz` is too large, download in [mosesdecoder](https://github.com/moses-smt/mosesdecoder).

## Referrence

Main referrence:

[Chinese-to-English translation based on Transformer](https://aistudio.baidu.com/projectdetail/2496060?channelType=0&channel=0)
