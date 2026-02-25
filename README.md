# Computer-Vision

A comparision of Transformer and CNN models over RGB satellite imagery
This workflow is detailed study of how different architecture behave on high resolution dataset.

`````````````````````````````````````````````````````````````````````````````````````
🛰 Dataset Details

Total samples: 500 image–mask pairs

Image resolution: 512 × 512

Number of classes: 5 (as available in the dataset)

Task: Pixel-wise semantic segmentation

Data split: Train / Validation 

Each mask contains integer-encoded class labels corresponding to five semantic land-cover categories.
``````````````````````````````````````````````````````````````````````````````````````
🧠 Models Compared
1️⃣ ResNet50-based Segmentation

Backbone: ResNet50

Encoder-decoder architecture

Pretrained weights used for initialization

Fine-tuned on satellite dataset

2️⃣ ResNet101-based Segmentation

Deeper backbone than ResNet50

Higher representational capacity

Increased parameter count

3️⃣ SegFormer B0

Transformer-based segmentation architecture

Efficient attention mechanism

Strong performance on dense prediction tasks 
````````````````````````````````````````````````````````````````````````````````````````````
⚙️ Training Configuration
🔹 Input Size

512 × 512

🔹 Loss Function

Cross-Entropy Loss



🔹 Optimizer

Adam / AdamW

🔹 Learning Rate Strategy

Tuned across multiple values

Scheduler applied (if used)

🔹 Batch Size

4

🔹 Epochs:10

(Insert value)

🔬 Hyperparameter Tuning

Hyperparameters tuned:

Learning rate: 1e-7

Batch size : 4

Optimizer selection :  adam

Best configurations were selected based on validation performance.
```````````````````````````````````````````````````````````````````````````````````````````
📊 Evaluation Metrics

Models were evaluated using:

Pixel Accuracy

Mean Intersection over Union (mIoU)

Confusion Matrix

