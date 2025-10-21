---
title: Professor's work
draft: false
tags:
  - school
---
# Thermal Image translation for enhanced environmental perception at night
## **Aim → 
To improve night-time vision by converting infrared (IR) images (which work in dark conditions) into visible-spectrum (VI) images (which humans find easier to interpret), _without_ needing paired IR-VI image datasets.
## Method →
They propose a framework called **IR2VI**, based on unsupervised Generative Adversarial Networks (GANs). Key additions:
- A _structure-connection module_ in the generator to preserve the original image’s structural information (so objects stay in correct shape/position) [CVF Open Access+1](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w21/Liu_IR2VI_Enhanced_Night_CVPR_2018_paper.pdf?utm_source=chatgpt.com)
- A _region-of-interest (ROI) focal loss_ (which includes ROI cycle-consistency and ROI adversarial loss) to pay special attention to important small objects and fine detail. [CVF Open Access](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w21/Liu_IR2VI_Enhanced_Night_CVPR_2018_paper.pdf?utm_source=chatgpt.com)  
    This lets the model learn mappings from IR to VI domain without exact pixel-to-pixel correspondence.
## **Why is this work better than conventional methods →**
- Many earlier methods either required _paired IR-VI images_ (which are very hard to obtain at night) or produced poor detail/incorrect mapping when only unpaired data was available. [arXiv+1](https://arxiv.org/abs/1806.09565?utm_source=chatgpt.com)

- IR2VI addresses _“incorrect mapping”_ (objects appear wrong) and _“lack of fine detail”_ (small objects get lost) by the added structure-connection and ROI loss modules. [CVF Open Access](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w21/Liu_IR2VI_Enhanced_Night_CVPR_2018_paper.pdf?utm_source=chatgpt.com)

- The unsupervised approach means it’s more practical for real night-vision applications where you don’t have ideal paired datasets.
## **Results →**
- Qualitative results: IR2VI produced translated visible-style images that maintained correct structures, clearer object boundaries, and richer detail versus baseline GAN translation methods. [CVF Open Access+1](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w21/Liu_IR2VI_Enhanced_Night_CVPR_2018_paper.pdf?utm_source=chatgpt.com)
    
- Quantitative evaluation: Using no-reference image quality metrics (e.g., NIQE, BRISQUE), and also object-detection performance on generated visible images, IR2VI outperformed several state-of-the-art unpaired image-translation methods. [arXiv](https://arxiv.org/abs/1806.09565?utm_source=chatgpt.com)
    
- For example: object detection AP (average precision) on generated images was much higher for their method versus alternatives. [arXiv](https://arxiv.org/abs/1806.09565?utm_source=chatgpt.com)
## **Conclusion →**  
IR2VI shows that unsupervised IR-to-VI translation _is practical_ and can significantly enhance environmental perception at night (especially when visible light is absent). The structure-connection and ROI focal loss are key innovations to overcome earlier limitations. The authors suggest future work could include more joint datasets or improved colorization steps. [CVF Open Access+1](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w21/Liu_IR2VI_Enhanced_Night_CVPR_2018_paper.pdf?utm_source=chatgpt.com)



# Enhanced situation awareness through CNN-based deep multimodal image fusion
## **Aim ->
To improve how well a system (e.g., for surveillance or autonomous vehicles) can “see” a scene by combining multiple image types (like visible-light + infrared) using deep learning, so that even in difficult conditions (night, fog) it can still detect objects clearly.
## **Method →
- They use a **deep convolutional neural network (CNN)** that takes images from different sensors (multimodal) — for example one visible image + one infrared image.
- The network fuses those modalities **early** or **mid-way** (not just after separate processing) so it learns **joint features** (things that matter in both IR and visible).
- They train the model so that the fused image or fused feature map gives better detection / awareness (objects, obstacles) rather than treating each image separately then combining results.
## **Why is this work better than conventional →
- Conventional methods often process each image modality separately (visible and IR) and then just merge or overlay results → that can lose subtle information or conflicting cues.
- The new approach fuses the modalities inside the deep network, allowing the model to learn _what parts of each modality are important together_, improving robustness.
- Especially in “hard” scenes (low light, obscured, thermal vs visible mismatch) conventional fusion fails or gives poor detail; this method gives better clarity and detection performance.
## **Results →
- Qualitative: The fused images / feature representations look clearer, with better object boundaries and less noise (especially in challenging lighting).
- Quantitative: They show improved metrics for object detection / classification / segmentation in the fused output compared to baseline visible-only, IR-only, or naive fusion methods.
- Real-world scenario experiments demonstrate that the model yields higher “situation awareness” (detect more objects reliably under bad conditions).
## **Conclusion →
The paper shows that CNN-based deep multimodal fusion is a **practical and effective** way to enhance visual awareness by leveraging multiple sensors. It outperforms simpler fusion techniques and repeatedly gives better detection/clarity in challenging scenes. The authors recommend future work on better sensor calibration, more modalities (e.g., radar, LIDAR) and real-time deployment.




# AIS DATA-DRIVEN GENERAL VESSEL DESTINATION PREDICTION: A TRAJECTORY SIMILARITY-BASED APPROACH

## **Aim →**  
To predict the destination port of a vessel using its AIS (Automatic Identification System) trajectory data in a general, global way — not just region-specific — so that we can tell _where the ship is going_ from its movement pattern.
## **Method →**
- Extract historical vessel trajectories from over 141 million AIS records (covering ~5.9 million trajectories) and the departure port information. [Open Collections](https://open.library.ubc.ca/cIRcle/collections/24/24/items/1.0380888?utm_source=chatgpt.com)
- Measure similarity between a current vessel’s trajectory and historical ones, using different similarity metrics.
- Use a Random Forest model combined with a “port frequency-based” decision strategy: the most similar past trajectories + frequency of destination ports are used to pick the predicted destination. [Open Collections](https://open.library.ubc.ca/cIRcle/collections/24/24/items/1.0380888?utm_source=chatgpt.com)
## **Why is this work better than conventional →**
- Conventional methods often focus only on **regional** destination prediction (limited set of ports) whereas this method is **general** (global port set). [Open Collections](https://open.library.ubc.ca/cIRcle/collections/24/24/items/1.0380888?utm_source=chatgpt.com)
- Many prior works use AIS data in simpler ways (e.g., only departure + speed) or have smaller datasets. This thesis uses **massive dataset** + advanced similarity + machine learning model → higher accuracy.
- The combination of trajectory similarity + decision strategy enables better prediction for “unknown” routes rather than just ones seen often.
## **Results →**
- On 35,937 test trajectories, the Random-Forest + port-frequency strategy achieved best accuracy compared to eight existing similarity methods with two decision strategies. [Open Collections](https://open.library.ubc.ca/cIRcle/collections/24/24/items/1.0380888?utm_source=chatgpt.com)
- Demonstrated that the method generalizes well across the wide dataset, showing improved prediction reliability.
## **Conclusion →**  
A data-driven approach using large AIS trajectory data + similarity metrics + machine learning (Random Forest) produces a strong general destination prediction system for vessels. The work suggests that with more real-time updating and even more data, such methods could support maritime traffic decision-making and safety more effectively.


