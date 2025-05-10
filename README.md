

# DenseNet201-SE with Explainable AI for Skin Lesion Classification

This repository presents a deep learning model developed as part of a research study titled:

**"Skin Lesion Classification with Explainable AI to Enhance Dermatological Diagnosis"**

The work integrates **DenseNet201 with Squeeze-and-Excitation (SE) blocks** and employs **Explainable AI (XAI)** techniques to classify skin lesions from MRI images. The model is trained and evaluated on the [PH² Skin Cancer MRI Dataset](https://www.kaggle.com/datasets/rashidul0/ph2-skin-cancer-classification), targeting more transparent and accurate clinical decision support.


## 🧠 Overview of the Model

Our architecture is grounded in **DenseNet201**, known for its efficient feature reuse and gradient flow. To improve discriminative ability, we embedded **SE blocks** that perform dynamic channel-wise feature recalibration, strengthening the network’s attention to informative features while suppressing noise.

The model architecture is enhanced further with **Explainable AI methods** such as Grad-CAM to visualize and understand the regions influencing model predictions. This promotes transparency and increases trustworthiness in clinical applications.


## 📂 Dataset Used

We utilize the **PH² Skin Lesion MRI Dataset**, which contains annotated dermatological images from clinical cases:

📌 [PH² Dataset on Kaggle](https://www.kaggle.com/datasets/rashidul0/ph2-skin-cancer-classification)

All images were resized, normalized, and augmented before feeding into the model.

---

## 💡 Key Contributions

- **DenseNet201-Backbone**: Powerful pre-trained feature extractor for medical imaging.
- **Squeeze-and-Excitation (SE) Blocks**: Attention mechanisms that adaptively emphasize important channels.
- **Explainability with Grad-CAM**: Post-hoc visualization to identify lesion regions critical for classification.
- **3-Class Diagnostic Support**: Accurate prediction across common lesion categories.
- **End-to-End Pipeline**: Preprocessing, training, evaluation, and explanation in one modular codebase.

---

## 🚀 How to Use

Clone the repo and install dependencies:

```bash
git clone https://github.com/your-username/skin-lesion-densenet201-se-xai.git
cd skin-lesion-densenet201-se-xai
pip install -r requirements.txt
````

To train:

```bash
python train.py --epochs 30 --batch_size 32
```

To generate XAI visualizations:

```bash
python grad_cam.py --image sample.jpg --model saved_model.pth
```

---

## 🤝 Contributions Welcome

We invite researchers, students, and developers interested in medical AI to contribute to this project. Whether you're exploring better attention mechanisms, alternative explainability techniques, or even deployment tools, your ideas are welcome!

To contribute:

1. Fork the repo.
2. Create a feature branch.
3. Submit a pull request with your changes.

For academic collaboration or integration into clinical pipelines, please contact us directly.

---

## 📜 License

This research code is released under the MIT License.

**Maintained by**: Bakary Gibba
**Institution**: Albukhary International University
**Field**: AI for Medical Imaging and Diagnostics

```
