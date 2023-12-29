Dive into the respective code files for more details.

## Structure

For the model paramter files too large to store, the files in related directories are empty for referrence.

```bash
.
├── data # dataset
│   ├── cat_12_test.zip
│   ├── cat_12_train.zip
│   └── train_list.txt
├── model # model paramter files
│   ├── cnn
│   │   └── final.pdparams
│   ├── gan
│   │   ├── final.pdparams # classifyer
│   │   ├── discriminator.pdmodel
│   │   └── generator.pdmodel
│   └── transformer
│       └── final.pdparams
├── pretrained_models # pretrained models
│   ├── dcgan
│   │   ├── discriminator.pdmodel
│   │   └── generator.pdmodel
│   └── resnet50
│       └── ResNet50_pretrained
├── cnn.ipynb # cnn code
├── transformer.ipynb # transformer code
├── gan.ipynb # gan code
├── visualdl # visual logs
│   ├── cnn
│   │   └── cnn.log
│   ├── gan
│   │   ├── gan.log
│   │   └── classifyer.log
│   └── transformer
│       └── transformer.log
└── submit.csv # file to submit for the game

```

## Attention

Dataset is too large, download in [Dataset of Cat Twelve Categories](https://aistudio.baidu.com/datasetDetail/10954).

## Referrence

Main referrence:

[Experience Competition of Cat Twelve Categories](https://aistudio.baidu.com/competition/detail/136/0/introduction)

[Baseline of Experience Competition of Cat Twelve Categories](https://aistudio.baidu.com/projectdetail/4243146)

[ViT (Vision Transformer) in paddle](https://paddlepedia.readthedocs.io/en/latest/tutorials/computer_vision/classification/ViT.html)
