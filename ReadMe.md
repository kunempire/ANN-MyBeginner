There are three tasks based on **Artificial Neural Network**: cats classifying, Chinese-news-titles classifying and translation from Chinese to English.

## Origin

Cats classifying focuses on image processing and Chinese-news-titles classifying focuses on NLP (Natural Language Processing), which are the main topic in machine learning. Also, classifying is a fundamental task, derived many tasks including machine translation. As the final examination of the course, *Artificial Neural Network*, it is a good practice beginning with the two tasks and an additional task based on them.

CNN, Transformer and GAN are the most basic model, mechanisms of which deeply influence the more and more powerful model today. For every beginner like me, it is  a must to master them for further studying. Therefore, models in the tasks are all based on these basic models.

## Structure

Directorys `cat_classify`, `title_classify` and `translation` are respectively to the three tasks. The ReadMes and notebooks in them are in details.

## How GAN to Classify

The ReadMes and notebooks in every task directoy are exhaustive. I shouldn't have gone into too much detail here. However, 'how GAN to classify' confused me most when finishing the tasks, which is worth recording separately here.

As we know, GAN (Generative Adversarial Network) is mainly used in AIGC (AI-Generated Content). GAN consists of two networks: a generator and a discriminator. These two networks progress together through adversarial training, allowing the generator to generate realistic data, while the discriminator can distinguish between real data and the data generated by the generator.

In the application of GAN, we are more focused on obtaining a high-performance generator to generate content that meets the requirements, while discriminators are often overlooked. But it constantly sees through the works of the generator, which makes the fake images produced by the other party more and more realistic. The discriminator itself is a powerful neural network that also learns many essential features of the input image, which can be used to fine tune the discriminator into a classifier through model fine-tuning.

The specific method is as follows: first, train a GAN network using conventional methods to obtain a generator and discriminator; Then modify the classification header of the discriminator to meet the requirements of the classification task; Next, load the trained discriminator model for model fine-tuning; Finally, the classifier obtained by fine-tuning the discriminator is obtained.

Personally understanding, discriminator networks have mastered the ability to extract input features in adversarial learning. In the task of distinguishing between true and false, these features are combined with parameters to obtain true or false. In the classification task, these features are still important, but parameters can be fine tuned (like modifying the number of ouput classes/features) to combine and obtain categories.

## Thanks

Sincere thanks to lively lectures of the professor and the patient guidance of teaching assistant in *Artificial Neural Network*.