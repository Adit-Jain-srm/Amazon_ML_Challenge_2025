# Amazon ML Challenge 2025 - Smart Product Pricing

## 🏆 Team Arize

**Team Members:**
- **Adit Jain** - Team Leader & Project Manager
- **Mehir Singh** - Data Scientist & Feature Engineer  
- **Ayush Pandey** - Model Developer & Vibes bringer
- **Adarsh Verma** - ML Engineer & Deep Learning Specialist

---

## 📋 Challenge Overview

This repository contains our solution for the **Amazon ML Challenge 2025 - Smart Product Pricing Challenge**. The challenge involves developing a machine learning solution to predict optimal product prices based on product details, including text descriptions and images.

### Problem Statement
In e-commerce, determining the optimal price point for products is crucial for marketplace success and customer satisfaction. Our task is to build a model that analyzes product details holistically and suggests an optimal price based on complex relationships between product attributes like brand, specifications, and product quantity.

### Evaluation Metric
- **Primary Metric**: Symmetric Mean Absolute Percentage Error (SMAPE)
- **Target**: Minimize SMAPE score on the test dataset
- **Constraint**: Model must be MIT/Apache 2.0 licensed with ≤8B parameters

---

## 🗂️ Project Structure

```
Amazon_ML_Challenge_2025/
├── README.md                           # This file
├── PS.md                              # Problem statement
├── LICENSE                            # MIT License
├── requirements.txt                   # Python dependencies
├── submission.ipynb                   # Complete ML pipeline notebook
├── student_resource/                  # Main project directory
│   ├── dataset/                       # Dataset files
│   │   ├── train.csv                 # Training data (75k samples)
│   │   ├── test.csv                  # Test data (75k samples)
│   │   ├── sample_test.csv           # Sample test input
│   │   ├── sample_test_out.csv       # Sample output format
│   │   └── test_out.csv              # Generated predictions
│   ├── src/                          # Source code
│   │   ├── utils.py                  # Image download utilities
│   │   └── example.ipynb             # Example notebook
│   ├── sample_code.py                # Sample prediction code
│   └── Documentation_template.md     # Documentation template
└── .gitignore                        # Git ignore rules
```

---

## 📊 Dataset Description

### Features
1. **sample_id**: Unique identifier for each sample
2. **catalog_content**: Text field containing product title, description, and Item Pack Quantity (IPQ)
3. **image_link**: Public URL for product image download
4. **price**: Target variable (only available in training data)

### Dataset Size
- **Training Set**: 75,000 products with complete details and prices
- **Test Set**: 75,000 products for final evaluation

---

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Required packages (see requirements.txt)

### Installation
1. Clone the repository:
```bash
git clone https://github.com/your-username/Amazon_ML_Challenge_2025.git
cd Amazon_ML_Challenge_2025
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Quick Start

#### Option 1: Run Complete ML Pipeline (Recommended)
```bash
# Open and run the complete submission notebook
jupyter notebook submission.ipynb
```

#### Option 2: Run Sample Code
1. Navigate to the student_resource directory:
```bash
cd student_resource
```

2. Run the sample code to understand the data format:
```bash
python sample_code.py
```

#### Option 3: Download Images (Optional)
```python
from student_resource.src.utils import download_images
import pandas as pd

# Load data
df = pd.read_csv('student_resource/dataset/train.csv')
image_links = df['image_link'].tolist()

# Download images
download_images(image_links, 'images/')
```

---

## 🧠 Our Approach

### Methodology Overview
*[To be updated with our final approach]*

Our solution leverages both textual and visual features to predict product prices:

1. **Text Processing**: Extract features from catalog content using NLP techniques
2. **Image Processing**: Analyze product images using computer vision models
3. **Feature Engineering**: Combine textual and visual features with domain knowledge
4. **Model Training**: Train ensemble models for robust price prediction

### Key Innovations
- [ ] Multimodal learning combining text and image features
- [ ] Advanced feature engineering for product attributes
- [ ] Ensemble methods for improved prediction accuracy
- [ ] Robust preprocessing pipeline for data quality

---

## 📈 Model Performance

### Validation Results
*[To be updated with actual results]*

- **SMAPE Score**: [Pending]
- **Training Time**: [Pending]
- **Model Size**: [Pending]

---

## 📝 Usage

### Training the Model
```bash
# Run the complete pipeline in the submission notebook
jupyter notebook submission.ipynb

# Or run individual components
cd student_resource
python sample_code.py
```

### Making Predictions
```bash
# The submission notebook will automatically generate predictions
# Output file: student_resource/dataset/test_out.csv
```

### Expected Output Format
The output file should be a CSV with exactly 2 columns:
- `sample_id`: Unique identifier matching the test record
- `price`: Predicted price as a positive float value

---

## 📋 Submission Requirements

### Files to Submit
1. **test_out.csv**: Predictions file matching sample_test_out.csv format (auto-generated by submission.ipynb)
2. **Documentation**: 1-page document describing our approach (using Documentation_template.md)
3. **Code**: Complete solution including:
   - `submission.ipynb` - Complete ML pipeline notebook
   - `requirements.txt` - All dependencies
   - `student_resource/` - Source code and utilities

### Important Notes
- ⚠️ **No External Price Lookup**: Strictly prohibited to use external pricing data
- All predictions must be positive float values
- Model must comply with MIT/Apache 2.0 license
- Model size must not exceed 8 billion parameters

---

## 📚 Key Files Overview

- **`submission.ipynb`**: Complete ML pipeline with data exploration, feature engineering, model training, and prediction generation
- **`requirements.txt`**: All necessary Python packages and dependencies
- **`README.md`**: Comprehensive project documentation and setup guide
- **`PS.md`**: Formatted problem statement with all challenge details
- **`student_resource/dataset/`**: Training and test datasets
- **`student_resource/src/utils.py`**: Image downloading utilities

## 🤝 Contributing

This is a competition project. For questions or collaboration, please contact the team leader.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🏅 Competition Timeline

- **Day 1**: Problem statement and dataset release
- **Day 2**: Model development and training
- **Day 3**: Final submissions and leaderboard reveal

---

## 📞 Contact

**Team Leader**: Adit Jain  
**Email**: aj9104@srmist.edu.in

---

*Last Updated: January 2025*
*Challenge Period: Amazon ML Challenge 2025*