# garbage-classfication
This project classifies waste into 10 categories: cardboard, battery, metal, paper, plastic, shoes, trash, biological, clothes, and glass. Using image recognition, the model improves waste sorting and recycling
efficiency, reducing environmental impact and supporting sustainable waste management.


📂 Dataset


The dataset used for this project is publicly available on Kaggle:
🔗 Garbage Classification Dataset

It contains images grouped into the following 10 categories:

Battery
Biological
Cardboard
Clothes
Glass
Metal
Paper
Plastic
Shoes
Trash
⚠️ Challenges with the Dataset
The dataset was not originally provided in CSV format.
It was not split into training and testing sets, so we had to manually organize it.
The dataset size was very small, which led to overfitting during initial training.
There was confusion between similar classes, such as transparent plastic vs. glass.
✅ Solutions Applied
Used data augmentation (flipping, rotation, zoom, etc.) to increase training data.
Applied fine-tuning on pretrained models to improve class distinction.
## 🧠 Model Comparison

We experimented with different CNN architectures for garbage classification:

| Model        | Pros                                                                 | Cons                        | Notes                                |
|--------------|----------------------------------------------------------------------|-----------------------------|--------------------------------------|
| **ResNet**   | 🔹 Very powerful <br> 🔹 High accuracy                                | ❌ Heavy <br> ❌ Large size  | Suitable for high-compute environments |
| **EfficientNet** | 🔹 Balanced performance <br> 🔹 Good accuracy-to-size ratio          | ❌ Slower than MobileNetV2  | Good trade-off for general use        |
| **MobileNetV2** ✅ | 🔹 Lightweight <br> 🔹 Fast <br> 🔹 High accuracy <br> 🔹 Fewer parameters | –                           | ✅ Final choice <br> Best for mobile/edge deployment |

👉 **Final Choice: MobileNetV2**  
Lightweight, accurate, and suitable for deployment on mobile and edge devices.

🚀 How to Use
🔴 Live Web App
Use our demo on Hugging Face Spaces:

[👉 Try it Live](https://644ccd78a5191b3e5d.gradio.live/)


📓 Notebook
[view on kaggle](https://www.kaggle.com/code/moazmohamed545/notebookd474f18c4a/edit)


prepeard by 
moaz mohamed 

[linkdin](https://www.linkedin.com/in/moaz-mohamed-545725375/)
