# Latest-development-of-ISR-VSR #
Mainly ICCV, ECCV and CVPR about ISR and VSR, especially lasted two years developments.

<!-- TOC -->

![](https://img.shields.io/badge/updated-today-brightgreen.svg) [***Unsupervised Super-resolution Method***](#Unsupervised-Super-resolution-Method)

<!-- TOC -->

There are some useful repositories thst help me a lot：  
1、[A collection of state-of-the-art video or single-image super-resolution architectures, reimplemented in tensorflow.](https://github.com/LoSealL/VideoSuperResolution) which has most great papers/models about ISR and VSR. Include some useful tools: some models with pre-trained weights, link of datasets, VSR package which offers a training and data processing framework based on TF or pytorch.  
2、[Video-Super-Resolution](https://github.com/flyywh/Video-Super-Resolution) which has some VSR paper's informations.

Thanks them. But above repositories are not completely, and most of ECCV2018 and CVPR2018 are not listed as well as my under-graduation project is doing, therefore, this repositories exists. (help me and you) I help it will be updating under our contributions.

If you think it is useful, please star it and spread it. Thank you.  
(Although the table is ugly)

## ISR: ##
<table>
    <tr>
        <th>abbreviation</th>
	<th>full name</th>
	<th>published</th>
	<th>code</th>
	<th>description</th>
	<th>keywords</th>
	<th>in undergraduationt*</th>
    </tr>
    <tr>
        <td>SRCNN</td>
        <td>Image Super-Resolution Using Deep Convlutional Network</td>
        <td>ECCV2014</td>
		<td>keras：https://github.com/qobilidop/srcnn</td>
        <td>has two version 2014 and ex-2016. Milestone in deep learning about SR.Simple three CNN network：patch extraction and representation, non-linear mapping and reconstraction</td>
		<td>Loss:MSE CNN</td>
        <td>*</td>
    </tr>
    <tr>
        <td>FSRCNN</td>
        <td>Accelerating the Super-Resolution Convolutional Neural Network</td>
        <td>ECCV2016</td>
		<td>official:matlab,caffe：http://mmlab.ie.cuhk.edu.hk/projects/FSRCNN.html</td>
        <td>Develop SRCNN, add deconv, input image don't need to upsample by bicubic and fine-tune accelerate</td>
		<td>deconvolution fine-tuninig last deconv</td>
        <td>*</td>
    </tr>
    <tr>
        <td>ESPCN</td>
        <td>Real-Time Single Image and Video Super-Resolution Using an Efficient Sub-Pixel Convolutional Neural Network</td>
        <td>CVPR2016</td>
		<td>github(tensorflow): https://github.com/drakelevy/ESPCN-TensorFlowhttps://
		github(pytorch): https://github.com/leftthomas/ESPCNhttps://
		github(caffe): https://github.com/wangxuewen99/Super-Resolution/tree/master/ESPCNhttps://</td>
        <td>A new way to upsamping: sub-pixel</td>
		<td>sub-pixel Tanh instead Relu Real time</td>
        <td>*</td>
    </tr>
	<tr>
        <td>VDSR</td>
        <td>Accurate Image Super-Resolution Using Very Deep Convolutional Networks</td>
        <td>CVPR2016</td>
		<td>"code: https://cv.snu.ac.kr/research/VDSR/
		github(caffe): https://github.com/huangzehao/caffe-vdsrhttps://
		github(tensorflow): https://github.com/Jongchan/tensorflow-vdsrhttps://
		github(pytorch): https://github.com/twtygqyy/pytorch-vdsrhttps://"</td>
        <td>Add residual, padding 0 every layer, scale mixture training</td>
		<td>"residual network
	Deep"</td>
        <td>*</td>
    </tr>
    <tr>
        <td>DRCN</td>
        <td>Deeply-Recursive Convolutional Network for Image Super-Resolution</td>
        <td>CVPR2016</td>
		<td>"code: https://cv.snu.ac.kr/research/DRCN/
		github(tensorflow): https://github.com/jiny2001/deeply-recursive-cnn-tfhttps://"</td>
        <td>"Learn RNN to add recursive and skip
		input image is interpolation image"</td>
		<td>"Recursive Neural Network
		Recursive Neural Network"</td>
        <td>*</td>
    </tr>
    <tr>
        <td>RED</td>
        <td>Image Restoration Using Convolutional Auto-encoders with Symmetric Skip Connections</td>
        <td>NIPS2016</td>
		<td>…</td>
        <td>Encoder-decoder and skip</td>
		<td>Encoder-decoder</td>
        <td>*</td>
    </tr>
    <tr>
        <td>DRRN</td>
        <td>Image Super-Resolution via Deep Recursive Residual Network</td>
        <td>CVPR2017</td>
		<td>github(caffe): https://github.com/tyshiwo/DRRN_CVPR17</td>
        <td>combine resNet and recursive</td>
		<td>"residual networkrecursive"</td>
        <td>*</td>
    </tr>
    <tr>
        <td>LapSRN</td>
        <td>Deep Laplacian Pyramid Networks for Fast and Accurate Super-Resolution</td>
        <td>CVPR2017</td>
		<td>"github(matconvnet): https://github.com/phoenix104104/LapSRN
		github(pytorch): https://github.com/twtygqyy/pytorch-LapSRNhttps:/
		github(tensorflow): https://github.com/zjuela/LapSRN-tensorflowhttps:/"</td>
        <td>Pyramid network new loss to constrain</td>
		<td>"Pyramid networkHuber loss"</td>
        <td>*</td>
    </tr>
<tr>
        <td>SRDenseNet</td>
        <td>Image Super-Resolution Using Dense Skip Connections </td>
        <td>ICCV2017</td>
		<td>"pytorch:
			https://github.com/wxywhu/SRDenseNet-pytorch"</td>
        <td>add dense block to model</td>
		<td>dense block</td>
        <td>*</td>
    </tr>

<tr>
        <td>SRGAN</td>
        <td>Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network</td>
        <td>CVPR2017</td>
		<td>"github(tensorflow): https://github.com/zsdonghao/SRGANhttps://
		github(tensorflow): https://github.com/buriburisuri/SRGANhttps://
		github(torch): https://github.com/junhocho/SRGANhttps:/AN
		github(caffe): https://github.com/ShenghaiRong/caffe_srganhttps:///caffe_srgan
		github(tensorflow): https://github.com/brade31919/SRGAN-tensorflowhttps://RGAN-tensorflow
		github(keras): https://github.com/titu1994/Super-Resolution-using-Generative-Adversarial-Networks
		https://er-Resolution-using-Generative-Adversarial-Networks
		github(pytorch): https://github.com/ai-tor/PyTorch-SRGAN"
	</td>
        <td>1st proposed GAN</td>
		<td>GAN</td>
        <td>*</td>
    </tr>

<tr>
        <td>EDSR(workshop)</td>
        <td>Enhanced Deep Residual Networks for Single Image Super-Resolution</td>
        <td>CVPR2017</td>
		<td>"github(torch): https://github.com/LimBee/NTIRE2017https://2017
		github(tensorflow): https://github.com/jmiller656/EDSR-Tensorflowhttps://
		github(pytorch): https://github.com/thstkdgus35/EDSR-PyTorchhttps://"</td>
        <td>remove BN</td>
		<td>"no BN MDSR"</td>
        <td>*</td>
    </tr>

<tr>
        <td>WDSR</td>
        <td>Wide Activation for Efficient and Accurate Image Super-Resolution</td>
        <td>arxiv2018</td>
		<td>pytorch：https://github.com/JiahuiYu/wdsr_ntire2018</td>
        <td>widen feature map and WN</td>
		<td>weight normalization</td>
        <td>*</td>
    </tr>

<tr>
        <td>SRMD</td>
        <td>Learning a Single Convolutional Super-Resolution Network for Multiple Degradations</td>
        <td>CVPR2018</td>
		<td>"matlab：
		https://github.com/cszn/SRMD"</td>
        <td>Degraded Fuzzy Kernel and Noise Level</td>
		<td>Degraded Fuzzy Kernel and Noise Level</td>
        <td>*</td>
    </tr>

<tr>
        <td>RDN(oral)</td>
        <td>Residual Dense Network for Image Super-Resolution(CVPR 2018 Spotlight</td>
        <td>CVPR2018</td>
		<td>"official:
		https://github.com/yulunzhang/RDN"</td>
        <td>"bicubic downsampling, gaussian kernel
		feature fusing"</td>
		<td>local and global Residual</td>
        <td>*</td>
    </tr>

<tr>
        <td>DBPN</td>
        <td>Deep Back-Projection Networks For Super-Resolution</td>
        <td>CVPR2018</td>
		<td>"pytorch:
		https://github.com/alterzero/DBPN-Pytorch"</td>
        <td>repeat down and up sample a back mechanism</td>
		<td>Back-Projection</td>
        <td>*</td>
    </tr>

<tr>
        <td>ZSSR</td>
        <td>“Zero-Shot” Super-Resolution using Deep Internal Learning(2018 CVPR</td>
        <td>CVPR2018</td>
		<td>"pytorch:
		https://github.com/jacobgil/pytorch-zssr"</td>
        <td>re-sample train test</td>
		<td>internally train</td>
        <td>*</td>
    </tr>

<tr>
        <td>SFTGAN</td>
        <td>Recovering Realistic Texture in Image Super-resolution by Deep Spatial Feature Transform</td>
        <td>CVPR2018</td>
		<td>"pytorch:
		https://github.com/xinntao/CVPR18-SFTGAN"</td>
        <td>semantic probability</td>
		<td>"semantic SFT"</td>
        <td>*</td>
    </tr>

<tr>
        <td>EUSR(workshop)</td>
        <td>Deep Residual Network with Enhanced Upscaling Module for Super-Resolution</td>
        <td>CVPR2018</td>
		<td>…</td>
        <td>change EDSR to EUSR by adding EUM</td>
		<td>enhanced upscaling module (EUM)</td>
        <td>*</td>
    </tr>

<tr>
        <td>CARN</td>
        <td>Fast, Accurate, and Lightweight Super-Resolution with Cascading Residual Network </td>
        <td>ECCV2018</td>
		<td>"pytorch:
		https://github.com/nmhkahn/CARN-pytorch"</td>
        <td>cascading block</td>
		<td>fast</td>
        <td>*</td>
    </tr>

<tr>
        <td>GAN_degradation</td>
        <td>To learn image super-resolution, use a GAN to learn how to do image degradation first </td>
        <td>ECCV2018</td>
		<td>…</td>
        <td>use GAN to prodecu LR near to nature</td>
		<td>mainly face test</td>
        <td>*</td>
    </tr>

<tr>
        <td>EPSR(workshop)</td>
        <td>Analyzing Perception-Distortion Tradeoff using Enhanced Perceptual Super-resolution Network</td>
        <td>ECCV2018</td>
		<td>...</td>
        <td>has a new metrics idea</td>
		<td>...</td>
        <td>*</td>
    </tr>
<tr>
        <td>SRFBN</td>
        <td>Feedback Network for Image Super-Resolution</td>
        <td>CVPR2019</td>
		<td>pytorch:https://github.com/Paper99/SRFBN_CVPR19</td>
        <td>feedback and a lot of comparation</td>
		<td>feedback</td>
        <td>/</td>
    </tr>

<tr>
        <td>RankSRGAN</td>
        <td>RankSRGAN: Generative Adversarial Networks with Ranker for Image Super- Resolution</td>
        <td>ICCV2019</td>
		<td>github:https://github.com/WenlongZhang0724/RankSRGANfocus</td>
        <td>focus on perceptual quality, and new method to use perceptual metrics named Ranker</td>
		<td>RankerRanker, RAN</td>
        <td>/</td>
    </tr>
    
<tr>
        <td>IMDN</td>
        <td>Lightweight Image Super-Resolution with Information Multi-distillation Network</td>
        <td>ACM MM2019</td>
		<td>github: https://github.com/Zheng222/IMDN</td>
        <td>todo:</td>
		<td>...</td>
        <td>/</td>
    </tr>

<tr>
        <td>RankSRGAN</td>
        <td>...</td>
        <td>...</td>
		<td>...</td>
        <td>...</td>
		<td>...</td>
        <td>/</td>
    </tr>

</table>

## VSR ##
<table>
	<tr>
        <th>abbreviation</th>
		<th>full name</th>
		<th>published</th>
		<th>code</th>
		<th>description</th>
		<th>keywords</th>
		<th>in undergraduation*</th>
    </tr>

<tr>
		<td>BRCN</td>
		<td>Bidirectional Recurrent Convolutional Networks for Multi-Frame Super-Resolution</td>
		<td>NIPS2015</td>
		<td>matlab:
			https://github.com/linan142857/BRCN</td>
		<td>It has three conv. Feedforward conv, recurrent conv and conditioned conv. And two sub-network: forward and backward sub-network</td>
		<td>Two sub-network and three kind conv
		use recurrent</td>
		<td>*</td>
	</tr>

<tr>
		<td>VESPCN</td>
		<td>Real-Time Video Super-Resolution with Spatio-Temporal Networks and Motion Compensation</td>
		<td>CVPR2017</td>
		<td>"pytorch:
		https://github.com/JuheonYi/VESPCN-PyTorch
		tensorflow:
		https://github.com/JuheonYi/VESPCN-tensorflow"</td>
		<td>compensation transformer: compare early fusion, slow fusion and 3D conv.</td>
		<td>"sub-pixel for video
	compensation transformer"</td>
		<td>*</td>
	</tr>

<tr>
		<td>SPMC</td>
		<td>Detail-revealing Deep Video Super-resolution</td>
		<td>ICCV2017</td>
		<td>"tensorflow:
		https://github.com/jiangsutx/SPMC_VideoSR"</td>
		<td>"show that proper frame alignment and motion compensation is crucial for achieving high quality results
		It includes motion estimate, SPMC layer and Detail Fusion Net"</td>
		<td>SPMC:  Subpixel Motion Compensation layer</td>
		<td>*</td>
	</tr>

<tr>
		<td>BRCN</td>
		<td>Bidirectional Recurrent Convolutional Networks for Multi-Frame Super-Resolution</td>
		<td>NIPS2015</td>
		<td>matlab:
			https://github.com/linan142857/BRCN</td>
		<td>It has three conv. Feedforward conv, recurrent conv and conditioned conv. And two sub-network: forward and backward sub-network</td>
		<td>Two sub-network and three kind conv
		use recurrent</td>
		<td>*</td>
	</tr>

<tr>
		<td>FRVSR</td>
		<td>Frame-Recurrent Video Super-Resolution</td>
		<td>CVPR2018</td>
		<td>"official:
		https://github.com/msmsajjadi/FRVSR"</td>
		<td>"we use a recurrent approach that passes the previously estimated HR frame as an input for the following iteration.
		Model includes Fnet and SRNet"</td>
		<td>"Flow estimation 
		Upscaling flow
		Warping previous output
		Mapping to LR space
		Super-Resolution
		Warp"
		</td>
		<td>*</td>
	</tr>

<tr>
		<td>DUF</td>
		<td>Deep Video Super-Resolution Network Using Dynamic Upsampling Filters Without Explicit Motion Compensation</td>
		<td>CVPR2018</td>
		<td>"tensorflow:
		https://github.com/HymEric/VSR-DUF-Reimplement
		https://github.com/yhjo09/VSR-DUF"</td>
		<td>"propose a novel end-to-end deep neural network that generates dynamic upsampling filters and a residual image, which are computed depending on the local spatio-temporal neighborhood of each pixel to avoid explicit motion compensation.
		The model includes filter generation network and residual generation network"
		</td>
		<td>"Dynamic upsampling filter
		Residual Learning"</td>
		<td>*</td>
	</tr>
<tr>
        <td>RBPN</td>
        <td>Recurrent Back-Projection Network for Video Super-Resolution</td>
        <td>CVPR2019</td>
		<td>Pytorch：https://github.com/alterzero/RBPN-PyTorch</td>
        <td>...</td>
		<td>recurrent
encoder-decoder module</td>
        <td>/</td>
    </tr>

<tr>
        <td>EDVR</td>
        <td>EDVR: Video Restoration with Enhanced Deformable Convolutional Networks</td>
        <td>CVPR2019</td>
		<td>Pytorch: https://github.com/xinntao/EDVR</td>
        <td>proposed two specify modules: PCD and TSA. PCD is for alignment and STA is for fusion. With deformable convolution, self-ensemble and two-stage redfine, it  wins all four tracks in the NTIRE19 Challenges for Video</td>
		<td>PCD:Pyramid, Cascading and Deformable (PCD) alignment module, TSA:Temporal and Spatial Attention fusion module</td>
        <td>/</td>
    </tr>
    
<tr>
        <td>Updating</td>
        <td>...</td>
        <td>...</td>
		<td>...</td>
        <td>...</td>
		<td>...</td>
        <td>/</td>
    </tr>
</table>


## Metrics dispute ##
Suggestion in SR: CVPR2018 ["The Perception-Distortion Tradeoff"](http://link.zhihu.com/?target=https%3A//arxiv.org/abs/1711.06077)

## Latest survey ##
arXiv2019: ["Deep Learning for Image Super-resolution: A Survey"](https://arxiv.org/abs/1902.06068)

## Upscale method ##
1. Dconvolution: ["Deconvolutional networks"](https://ftp.cs.nyu.edu/~fergus/papers/matt_cvpr10.pdf)
2. sub-pixel: ["Real-Time Single Image and Video Super-Resolution Using an Efficient Sub-Pixel Convolutional Neural Network"](https://arxiv.org/abs/1609.05158)
3. Unpooling: ["Visualizing and understanding convolutional networks"](https://arxiv.org/abs/1311.2901)
4. DUpsample: ["Decoders Matter for Semantic Segmentation: Data-Dependent Decoding Enables Flexible Feature Aggregation"](https://arxiv.org/abs/1903.02120)
5. carafe: ["CARAFE- Content-Aware ReAssembly of FEatures"](https://arxiv.org/abs/1905.02188)
6. meta-SR: ["Meta-SR-A Magnification-Arbitrary Network for Super-Resolution"](https://arxiv.org/abs/1903.00875)

## Unsupervised Super-resolution Method ##
1. [“Zero-Shot” Super-Resolution using Deep Internal Learning](http://openaccess.thecvf.com/content_cvpr_2018/html/Shocher_Zero-Shot_Super-Resolution_Using_CVPR_2018_paper.html), CVPR2018
2. [Unsupervised image super-resolution using cycle-in-cycle generative adversarial networks](http://openaccess.thecvf.com/content_cvpr_2018_workshops/w13/html/Yuan_Unsupervised_Image_Super-Resolution_CVPR_2018_paper.html), CVPRW2018
3. [Adversarial training with cycle consistency for unsupervised super-resolution in endomicroscopy](https://www.sciencedirect.com/science/article/pii/S1361841518305966), Medical image analysis 2019
4. [Self-Supervised Fine-tuning for Image Enhancement of Super-Resolution Deep Neural Networks](https://arxiv.org/abs/1912.12879), arXiv2019
5. [Unsupervised Learning for Real-World Super-Resolution](https://arxiv.org/abs/1909.09629), arXiv2019
6. [Unsupervised Single-Image Super-Resolution with Multi-Gram Loss](https://www.mdpi.com/2079-9292/8/8/833), MDPI2019

## Author ##
EricHym (Yongming He)  
Interests: CV and Deep Learning  
If you have or find any problems, this is my email: yongminghe@zju.edu.cn. And I'm glad to reply it. Thanks.  

Anyone can make contrbutions!
