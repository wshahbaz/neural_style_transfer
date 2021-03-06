# Neural Style Transfer
Neural Style Transfer model that combines a *content image* with a *style reference image* to yield artistic renders.

The result was achieved by optimizing a Style Content Model. In this model we preprocess the input on a pretrained VGG19 model (trained on imagenet), 
then extract the intermediate layer activations to obtain weight activations learned from our content image, followed by computing the style-content loss and
updating our model weights to acheive a smoother combined image.

## Example
Given as input content image and style reference image, respectively

<p>
<img src="https://c8.alamy.com/comp/TX4MAF/portrait-of-three-tame-alpacas-wearing-bow-ties-TX4MAF.jpg" height="300px" />
<img src="https://images.fineartamerica.com/images/artworkimages/mediumlarge/2/language-of-light-vesna-delevska.jpg" height="300px"/>
</p>

with neural style transfer we can generate image

![Neural Style Transfer Output](stylized-image.png)

### References
- [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576)
