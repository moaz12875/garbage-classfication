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


🧠 Model
We experimented with different CNN architectures:

Model	Pros / Cons
ResNet	Powerful but heavy
EfficientNet	Balanced performance and size
MobileNetV2	✅ Lightweight, ✅ Fast, ✅ High accuracy
✅ Final Choice: MobileNetV2
Low number of parameters
High accuracy
Suitable for mobile/edge deployment
