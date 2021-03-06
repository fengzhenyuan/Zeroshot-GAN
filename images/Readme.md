## Related work

Indeed there are some researchers have implemented the idea of **One-Shot** or **Zero-Shot**, however, the results are limited to the training set and they are not generative. For instance, the [cGAN-based Manga Colorization Using a Single Training Image](https://arxiv.org/pdf/1706.06918.pdf) is quite an amazing idea. Their result is obtained from using one single image as training set, which is of great simplicity. Here is their result
<img src="https://raw.githubusercontent.com/LinkWoong/Zeroshot-GAN/master/image.png" width="900px"/>  


--------------------------------------------------

In our project, we will generate chinese handwriting characters instead of colorization of images. It is more difficult to generate Chinese characters due to its complexity and abundance. In fact, the first level of Chinese characters including 3755 and second level contains 3008 characters. 

## Initial ideas

The very first thing that comes to my mind is using GAN and Convnets, their performance on different kinds of task is successful. Then why uses of small amount of data could learn the entire style of dataset? How this prediction is implemented?   
From the paper I've been reading through, I grabbed two gists for shrinking the size of training set. Indeed, some of the papers proposed an idea of **base**, which is used to generate the other characters. In 2016, there is a research group in Peking University implemented the 
[idea](http://delivery.acm.org/10.1145/3010000/3005371/a12-lian.pdf?ip=180.208.58.161&id=3005371&acc=ACTIVE%20SERVICE&key=BF85BBA5741FDC6E%2E92C009F8922DF942%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&CFID=813028674&CFTOKEN=68050724&__acm__=1506257565_0edf6f4190f7286c1f0b75a64016bc48). Their result is **1%** of the dataset
