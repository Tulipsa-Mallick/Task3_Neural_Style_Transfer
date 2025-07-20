# Task3_Neural_Style_Transfer
# 🎨 Neural Style Transfer with TensorFlow – Task 3 (Generative AI Internship)

Welcome to my implementation of **Neural Style Transfer (NST)**, part of **Task 5** under the **Generative AI Internship** offered by **Prodigy Infotech**. This project creatively blends the **content of one image** with the **style of another** to produce stunning visuals using deep learning. It’s an exciting combination of **art and AI**, using **convolutional neural networks (CNNs)** and **transfer learning**.


## 🧠 About Neural Style Transfer

Neural Style Transfer is a technique that uses **deep learning** to merge two images:

* The **content image** (which defines the objects/structure), and
* The **style image** (which defines colors, textures, and brushstrokes).

This method allows you to take a photo and "paint" it in the style of famous artworks, such as Van Gogh’s *Starry Night* or Picasso’s abstract style. It uses a **pre-trained CNN (VGG19)** to extract high-level features from both images and optimizes a new image to match content and style constraints.


## 🔍 Project Highlights

* ✅ Based on TensorFlow and Keras with pre-trained VGG19
* ✅ Applies **Gram Matrix** computations for style representation
* ✅ Separates **style loss** and **content loss** for better tuning
* ✅ Fine-tuned via **gradient descent optimization**
* ✅ Flexible for custom images (uploaded through Google Colab)
* ✅ Intuitive image visualizations and saving functionality



## 🧪 Technology Stack

* **Language**: Python 3
* **Libraries**:

  * TensorFlow / Keras
  * NumPy
  * Matplotlib
* **Model**: VGG19 (pre-trained on ImageNet)



## 🚀 How to Use It

You can run this project on **Google Colab** without any setup hassle.

### Step-by-Step:

1. **Open** the notebook in Google Colab.
2. **Upload** two images when prompted:

   * A content image (e.g., a portrait, scenery)
   * A style image (e.g., a painting or abstract art)
3. The notebook will process them and perform neural style transfer.
4. You will see intermediate results and the final stylized image.
5. Save or download the image output.

### You can also customize:

* num_iterations: Number of optimization steps (more = better quality)
* content_weight and style_weight: Control the influence of each image
* Optimizer learning rate (for speed vs quality)


## 💡 How It Works Internally

1. **Preprocessing**: Both content and style images are resized and normalized.
2. **Feature Extraction**: VGG19 is used to extract content and style features.
3. **Gram Matrices**: Style is captured via correlation between features.
4. **Loss Function**:

   * Content Loss: MSE between generated and content image features
   * Style Loss: MSE between generated and style image Gram matrices
   * Total Loss = α × Content Loss + β × Style Loss
5. **Optimization**: Generated image is updated iteratively using gradient descent.
6. **Postprocessing**: Final image is converted back to RGB for display.


## 📷 Example Visuals

| Content Image           | Style Image         | Stylized Output       |
| ----------------------- | ------------------- | --------------------- |
| ![content](content.jpg) | ![style](style.jpg) | ![output](output.png) |


## 📜 Result Interpretation

The result is a creative fusion where:

* The structure remains that of the content image.
* The color palette, texture, and brush strokes are adopted from the style image.

For example, a selfie could be painted in the style of *The Starry Night* or *The Scream*.



## 💼 Internship Details

* **Program**: Generative AI Internship
* **Company**: [Prodigy Infotech](https://prodigyinfotech.dev)
* **Task**: 03 – Neural Style Transfer using TensorFlow
* **Role**: Intern – AI/ML Developer
* **Tools Used**: Google Colab, TensorFlow, Keras, Matplotlib

This task helped me understand how convolutional networks can be repurposed for creative applications. It also improved my understanding of style loss, content representation, and optimization-based deep learning techniques.



## 📌 Key Learnings

* How to extract and compare deep visual features using CNNs
* Hands-on experience with TensorFlow and VGG19
* Optimization techniques and loss balancing
* Practical AI application in art generation



## 📃 License

This project is licensed under the **MIT License**.
You are free to reuse, share, and modify this code with proper attribution.


✨ Passionate about blending AI and Creativity!


The pictures which I used
Content Image - [load_img](https://github.com/user-attachments/assets/497bad4d-a396-4ebf-a84c-ba2a22261c73)
Style Image was inspired by Van Gogh as i can't upload it.
