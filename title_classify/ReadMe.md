Dive into the respective code files for more details.

## Structure

For the model paramter files too large to store, the files in related directories are empty for referrence.

```bash
.
├── data # dataset
│   ├── dev.txt
│   ├── test.txt
│   └── train.txt
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
│   ├── cnn
│   │   └── final.pdparams
│   ├── gan
│   │   ├── discriminator.pdmodel
│   │   └── generator.pdmodel
│   └── transformer
│       └── final.pdparams
├── result.txt # predict on test date set
├── submission.zip # file to submit for the game
├── transformer.ipynb # transformer code
├── cnn.ipynb # cnn code
├── gan.ipynb # gan code
├── visualdl # visual logs
│   ├── cnn
│   │   └── cnn.log
│   ├── gan
│   │   ├── gan.log
│   │   └── classifyer.log
│   └── transformer
│       └── transformer.log
└── vocabulary.json # vocabulary dictionary

```

## Referrence

Main referrence:

[Experience Competition for Chinese News Text Title Classification](https://aistudio.baidu.com/competition/detail/809/0/introduction)

[Baseline of Experience Competition for Chinese News Text Title Classification](https://aistudio.baidu.com/projectdetail/2311230)

[Text classification based on CNN](https://blog.csdn.net/weixin_45722572/article/details/126438740)
