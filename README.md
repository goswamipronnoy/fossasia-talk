# fossasia-talk
This repository contains additional reading material related to our presentation at the FossAsia conference.

## Abstract

The project aims at proposing a solution to restore underwater images for Marine Archeological studies. This work was done during a research internship at CSIR-National Institute of Oceanography. We worked with datasets provided by the field work and underwater explorations in the Arabian Sea along Western Coast of India. In this project, the traditional image restoration approach is extended by incorporating underwater optical properties into the system response function. Underwater turbidity causes loss of clarity transparency, visibility and the luminosity in underwater images to study a particular scene for Marine Archeologists. In this project, we have implemented and compared different methods of underwater image enhancement and restoration which are degraded by the turbidity in water. We implemented the various image processing algorithms considering an average quality camera (i.e., Logitech C920). The algorithms implemented in a step-wise manner are preprocessing, filtering, enhancement and denoising based on a model. Images tend to get degraded as the depth and turbidity increases, the amount of light on objects decreases and light distribution becomes nonuniform. To tackle this issue, the input images are converted to YCbCr color space and Contrast Limited Adaptive Histogram Equalization (CLAHE) is performed on the Luminescence(Y) channel of the image which improves the local contrast, at the same time limiting the amplification which can over-amplify the noise too. The filtering and enhancement were done using the Bilateral Filter and then finally the enhancement was carried out using the wavelet denoising method and de-blurring. Due to the intensity variations involved in underwater sensing, denoising is carefully carried out by wavelet decompositions. This is necessary to explore different effects of restoration constraints, and especially their response to an underwater environment where the effects of scattering can be easily treated as either signal or noise.

Since our solution aided the marine archeologists in their studies, we gave more emphasis to the information extraction and the visibility of features rather than the enhancing the physical features of the underwater images.
