# Ponymation: Learning 3D Animal Motions from Unlabeled Online Videos

[Keqiang Sun](https://keqiangsun.github.io/)<sup>1*</sup>, [Dor Litvak](https://dorlitvak.github.io)<sup>2,3*</sup>, [Yunzhi Zhang](https://cs.stanford.edu/~yzzhang/)<sup>2</sup>, [Hongsheng Li](https://www.ee.cuhk.edu.hk/~hsli/)<sup>1</sup>, [Jiajun Wu](https://jiajunwu.com)<sup>2†</sup>, [Shangzhe Wu](https://elliottwu.com)<sup>2†</sup>

<sup>1</sup>CUHK MMLab, <sup>2</sup>Stanford University, <sup>3</sup>UT Austin

(* Equal Contribution, † Equal Advising)


## Abstract

We introduce Ponymation, a new method for learning a generative model of articulated 3D animal motions from raw, unlabeled online videos. Unlike existing approaches for motion synthesis, our model does not require any pose annotations or parametric shape models for training, and is learned purely from a collection of raw video clips obtained from the Internet. We build upon a recent work, MagicPony, which learns articulated 3D animal shapes purely from single image collections, and extend it on two fronts. First, instead of training on static images, we augment the framework with a video training pipeline that incorporates temporal regularizations, achieving more accurate and temporally consistent reconstructions. Second, we learn a generative model of the underlying articulated 3D motion sequences via a spatio-temporal transformer VAE, simply using 2D reconstruction losses without relying on any explicit pose annotations. At inference time, given a single 2D image of a new animal instance, our model reconstructs an articulated, textured 3D mesh, and generates plausible 3D animations by sampling from the learned motion latent space.

## Video Presentation

<!-- [![Ponymation Video](https://img.youtube.com/vi/poc7c-9hCvQ/0.jpg)](https://www.youtube.com/watch?v=poc7c-9hCvQ) -->
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/poc7c-9hCvQ?si=TRMwwkQYrH4FTRfI"
  frameborder="0"
  allow="autoplay; encrypted-media"
  allowfullscreen
>
</iframe>

<!-- ## Motion Generation Results

Given just a single test image, we can generate diverse 4D animations in a feedforward fashion within seconds, including abstract drawings and artifacts.

![Motion Generation Example](assets/image_drive.mp4) -->

## BibTeX

```bibtex
@Article{sun2023ponymation,
  title     = {Ponymation: Learning 3D Animal Motions from Unlabeled Online Videos},
  author    = {Keqiang Sun and Dor Litvak and Yunzhi Zhang and Hongsheng Li and Jiajun Wu and Shangzhe Wu},
  journal   = {arXiv preprint arXiv:2312.13604},
  year      = {2023}
}