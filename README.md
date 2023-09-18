# Pix2Pix
A clean, simple and readable implementation of Pix2Pix in PyTorch.

## Results
The model was trained on the Maps dataset.
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/99168099/268786656-06e8d9e3-fa83-49fa-aa83-b29232b02fea.jpg">

### Training
Edit the config.py file to match the setup you want to use. Then run train.py

## Pix2Pix paper
### Image-to-Image Translation with Conditional Adversarial Networks by Phillip Isola, Jun-Yan Zhu, Tinghui Zhou, Alexei A. Efros

#### Abstract
We investigate conditional adversarial networks as a general-purpose solution to image-to-image translation problems. These networks not only learn the mapping from input image to output image, but also learn a loss function to train this mapping. This makes it possible to apply the same generic approach to problems that traditionally would require very different loss formulations. We demonstrate that this approach is effective at synthesizing photos from label maps, reconstructing objects from edge maps, and colorizing images, among other tasks. Indeed, since the release of the pix2pix software associated with this paper, a large number of internet users (many of them artists) have posted their own experiments with our system, further demonstrating its wide applicability and ease of adoption without the need for parameter tweaking. As a community, we no longer hand-engineer our mapping functions, and this work suggests we can achieve reasonable results without hand-engineering our loss functions either.
```
@misc{isola2018imagetoimage,
      title={Image-to-Image Translation with Conditional Adversarial Networks}, 
      author={Phillip Isola and Jun-Yan Zhu and Tinghui Zhou and Alexei A. Efros},
      year={2018},
      eprint={1611.07004},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

# Note
Training on custom dataset requires the above shown image format for the dataloader to properly create the dataset for training. The input and target images should be of the same dimensions and must be attached to each other.
