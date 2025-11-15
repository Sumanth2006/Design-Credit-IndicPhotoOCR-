Scene Text Data Collection & Evaluation Using IndicPhotoOCR

This project focuses on collecting images, writing text annotations, and using the existing IndicPhotoOCR system to understand how OCR works on real-world scene-text images.

We did not build any model.
We only used IndicPhotoOCR to test how well it reads text from our collected images.

What We Did

Collected real-world images containing Indian-language text

Wrote the correct text manually for each image

Used the existing IndicPhotoOCR toolkit to compare its OCR output with our annotations

Observed where the OCR system works well and where it struggles

Learned the flow of a simple ML pipeline through hands-on practice

Key Learnings

Basics of data collection

Importance of clean text annotations

How OCR behaves on different types of images

Practical challenges while handling scene-text images

Acknowledgement

We sincerely thank the IndicPhotoOCR team for providing the open-source OCR toolkit that we used in this project.
Toolkit Repository: https://github.com/Bhashini-IITJ/IndicPhotoOCR

Evaluation Script
>>> from IndicPhotoOCR.ocr import OCR
# Create an object of OCR
>>> ocr_system = OCR(verbose=True, identifier_lang ="auto") # for CPU --> OCR(device="cpu")
# Complete pipeline
>>> ocr_system.ocr("test_images/image_141.jpg")
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Recognized word: रोड
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Recognized word: बाराखम्बा
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Recognized word: राजीव
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Recognized word: चौक
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Recognized word: मण्डी
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Recognized word: हाऊस
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Using cache found in /root/.cache/torch/hub/baudm_parseq_main
# Recognized word: rajiv
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Using cache found in /root/.cache/torch/hub/baudm_parseq_main
# Recognized word: chowk
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Using cache found in /root/.cache/torch/hub/baudm_parseq_main
# Recognized word: mandi
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Using cache found in /root/.cache/torch/hub/baudm_parseq_main
# Recognized word: house
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Using cache found in /root/.cache/torch/hub/baudm_parseq_main
# Recognized word: barakhamba
# Identifying script for the cropped area...
# Recognizing text in detected area...
# Using cache found in /root/.cache/torch/hub/baudm_parseq_main
# Recognized word: road



Contributors

Tirunagari Bhuvan Sri Sai (B24BB1040)

Kesanapalli Jithin (B24CM1037)

Jeram Arjun (B24CM1034)

Gopi Sumanth Chadalavada (B24CM1084)
