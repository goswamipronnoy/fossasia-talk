# fossasia-talk
This repository contains additional reading material related to our presentation at the FossAsia conference.

## Abstract

The project aims at proposing a solution to restore underwater images for Marine Archaeological studies. This work is the outcome of the research done at *Council of Scientific & Industrial Research - National Institute of Oceanography (CSIR - NIO), Goa, India.* I worked with datasets provided by the field-work and underwater explorations in the Arabian Sea along Western Coast of India. In this project, the traditional image restoration approach is extended by incorporating underwater optical properties into the system response function. Underwater turbidity causes loss of clarity, transparency, visibility, and the luminosity in underwater images to study a particular scene for Marine Archaeologists. In this project, I have implemented and compared different methods of underwater image enhancement and restoration which are degraded by the turbidity in water. I implemented the various image processing algorithms considering an average quality camera (i.e., Logitech C920). The algorithms that are implemented in a stepwise manner are:
* **preprocessing**
* **filtering**
* **enhancement**
* **denoising based on a model**

Images tend to get degraded as the depth and turbidity increases. The amount of light on objects decreases and light distribution becomes non-uniform. To tackle this issue, the input images are converted to `YCbCr` color space and `Contrast Limited Adaptive Histogram Equalization (CLAHE)` is performed on the `luminescence (Y) channel` of the image which improves the local contrast, at the same time limiting the over-amplification of the noise. The filtering and enhancement were done using the bilateral filter and then finally the enhancement was carried out using the `wavelet denoising method` and de-blurring. Due to the intensity variations involved in underwater sensing, denoising is carefully carried out by wavelet decompositions. This is necessary to explore different effects of restoration constraints, and especially their response to an underwater environment where the effects of scattering can be easily treated as either signal or noise.

Since, the purpose of this project was to aid the marine archaeologists in their studies, more emphasis has been given to feature extraction and the information that they provide rather than the enhancing the physical features of the underwater images.

## Algorithm

! [Algorithm](https://drive.google.com/open?id=1HtoFk45ZE-HuSXLme3mjV_vhNdbvG1kR)
