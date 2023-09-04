# AI-based-image-segmentation-with-water-bodies-images-from-satellite-data

Dataset link: https://drive.google.com/file/d/1Zcr34N3hM0PrVnbUAwklLFtQuaE1mGvx/view?usp=sharing

UNet is a convolutional neural network (CNN) architecture commonly used for semantic segmentation tasks in computer vision. It was introduced by Olaf Ronneberger, Philipp Fischer, and Thomas Brox in 2015. UNet stands for "U-shaped network" because of its distinctive U-shaped architecture.

The main objective of semantic segmentation is to assign a class label to each pixel in an image, thereby segmenting the image into meaningful regions. UNet tackles this task by leveraging an encoder-decoder architecture, which allows it to capture both local and global context information.

![image](https://github.com/rahul13289/AI-based-image-segmentation-with-water-bodies-images-from-satellite-data/assets/97829880/e9d846cb-687a-4239-b93f-0b09594b5778)

Here's a breakdown of the UNet architecture:

1. **Encoder**: The encoder part of UNet consists of a series of convolutional and pooling layers. These layers progressively reduce the spatial dimensions of the input image while increasing the number of feature channels. This process helps extract hierarchical features from the input image, capturing both low-level and high-level information.

2. **Decoder**: The decoder part of UNet is a mirror image of the encoder. It consists of a series of upsampling and convolutional layers. The upsampling layers gradually increase the spatial dimensions of the feature maps while reducing the number of channels. These upsampling layers allow the network to recover spatial information lost during the encoding process. Additionally, skip connections are introduced between the corresponding encoder and decoder layers. These connections provide a shortcut for the network to transfer low-level spatial details from the encoder to the decoder.

3. **Bridge**: The bridge between the encoder and decoder is a single convolutional layer. It helps to connect the low-level and high-level features extracted by the encoder to the decoder.

4. **Output**: The final layer of UNet is a 1x1 convolutional layer that produces a segmentation map. This map has the same spatial dimensions as the input image, with each pixel assigned a class label indicating the predicted semantic segmentation.

UNet's U-shaped architecture allows it to capture both local details and global context, which is crucial for accurate semantic segmentation. The skip connections enable the network to recover fine-grained spatial information, while the encoder-decoder structure captures high-level contextual information.

UNet has been widely adopted and adapted for various segmentation tasks in medical imaging, satellite imagery analysis, and other domains where pixel-level segmentation is required. Its effectiveness, efficiency, and ability to handle limited training data have made it a popular choice in the field of computer vision.
