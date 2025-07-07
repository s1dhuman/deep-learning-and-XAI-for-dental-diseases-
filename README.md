# 🦷 **Deep Learning & Explainable AI for Dental Disease Detection** 🦷  

Rsearch Project as the part of B Tech Project (BTP)
*Automated diagnosis of 6 common dental conditions using lightweight AI*  

## 🚀 **Project Overview**  
We developed a **MobileNetV2-based architecture** to detect dental diseases from **colored photographic images** with:  
- **93.06% overall accuracy**  
- **Grad-CAM explainability** for clinical trust  
- **Mobile-friendly design** for real-world deployment  

## 🛠️ **How We Built It**  
1. **Benchmarked Models**  
   - Tested ResNet, EfficientViT, InceptionV3, VGG-16  
   - Chose **MobileNetV2** for its balance of speed/accuracy  

2. **Custom Architecture**  
   ```python  
   EnhancedMobileNetV2 +  
   ➔ Feature Pyramid Network (FPN)  
   ➔ Squeeze-and-Excitation (SE) Blocks  
   ➔ Transformer Encoder  
   ➔ Grad-CAM Visualization  
   ```

3. **Key Innovations**  
   - **Multi-scale detection** (tiny caries → large ulcers)  
   - **Channel attention** for color/texture patterns  
   - **Global context modeling** for spatial relationships  

## 📸 **Dataset**  
| **Metric**         | **Value**       |  
|---------------------|-----------------|  
| Total Images        | 34,410          |  
| Classes             | 6 (Caries, Calculus, Tooth Discoloration, Gingivitis, Ulcers, Hypodontia) |  
| Augmentation        | Flips, Rotations, Brightness |  
| Image Resolution    | 640x640 pixels  |  

## 📊 **Results Summary**  
| Disease           | Precision | Recall  | F1 Score | Support |  
|--------------------|-----------|---------|----------|---------|  
| **Ulcers**         | 0.9937    | 0.9795  | 0.9865   | 1607    |  
| **Caries**         | 0.9543    | 0.9746  | 0.9643   | 1970    |  
| **Discoloration**  | 0.9583    | 0.9462  | 0.9522   | 1116    |  
| **Hypodontia**     | 0.9583    | 0.9388  | 0.9485   | 294     |  
| **Gingivitis**     | 0.8952    | 0.7907  | 0.8397   | 994     |  
| **Calculus**       | 0.7066    | 0.8504  | 0.7719   | 575     |  
| **Overall**        | -         | -       | **0.9306** | 6556    |  

## 💡 **Why This Project?**  
- ✅ **Lightweight**: Runs efficiently on mobile devices  
- ✅ **Explainable**: Grad-CAM heatmaps show model decisions  
- ✅ **Scalable**: Handles diverse clinical imaging conditions  
- ✅ **Impact**: Addresses global dental health accessibility  

## 🏃♂️ **How to Run**  
### **Dependencies**  
```bash  
pip install tensorflow numpy matplotlib scikit-learn opencv-python jupyter  
```

### **Steps**  
1. **Download Dataset**  
   - Clone repo and unzip dataset into `/data` folder    ---> will upload dataset soon

2. **Run Notebook**  
   ```bash  
   jupyter notebook dental_diagnosis.ipynb  
   ```
   - **Training**: Uses GPU (recommended) with mixed precision  
   - **Evaluation**: Generates Grad-CAM visualizations automatically  

## 📬 **Contact**  
- **Team**: Jaya Sidhu Seelam, Eben Aby Eapen, Aditya Kabra, Dr. Gaurav Singal (NSUT, India)
