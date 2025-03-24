# Getting started with numpy.
Understand all the numpy basics in just 30 minutes. The one week work reduced to minutes for begginers who have knowledge in Python only. If you are are a beginner to numpy, then you are viewing the right notebook. 


# NumPy Basics for Beginners  
A hands-down guide to NumPy fundamentals through interactive Colab examples  

## Table of Contents  
1. **Installation & Setup**  
2. **Core Concepts**  
3. **Real-World Examples**  
4. **Next Steps**  

---

## 1. Installation & Setup  
```python  
# Install (if needed)  
!pip install numpy  

import numpy as np  
```  

---

## 2. Core Concepts  

### Creating Arrays  
```python  
# From lists  
numbers = np.array([1,2,3])  

# Special arrays  
zeros = np.zeros((2,3)  # 2x3 matrix of zeros  
ones = np.ones((3,2)     # 3x2 matrix of ones  
range_arr = np.arange(0,10,2)  # [0 2 4 6 8]  
```  

### Array Properties  
```python  
arr = np.array([[1,2,3],[4,5,6]])  
print(arr.shape)  # (2,3) dimensions  
print(arr.size)   # 6 elements  
print(arr.dtype)  # e.g., int32  
```  

### Basic Operations  
```python  
a = np.array([1,2,3])  
print(a + a)  # [2 4 6]  
print(np.sqrt(a))  # [1. 1.414 1.732]  
```  

### Aggregation  
```python  
temps = np.array([22.5, 23.7, 24.3, 21.8, 19.4])  
print(temps.mean())  # ~22.34  
print(np.median(temps))  # 22.5  
```  

---

## 3. Real-World Examples  

### Image Processing  
Convert RGB to grayscale:  
```python  
# Simulate image  
rgb = np.random.randint(0,256, (128,128,3))  

# Convert  
grayscale = np.mean(rgb, axis=2).astype(np.uint8)  

# Display (requires Matplotlib in next notebook)  
```  

### Stock Analysis  
Calculate daily price changes:  
```python  
stock_prices = np.array([...])  
changes = np.diff(stock_prices, axis=0)  # Compare rows  
```  

---

## 4. Next Steps  
**Next Notebook Topic**:  
`NumPy + Matplotlib Integration`  
- Visualize arrays with line plots  
- Create histograms/heatmaps  
- Overlay statistical data  

---

## Why NumPy?  
- **Speed**: 10-100x faster than lists  
- **Vectorization**: Perform operations on entire arrays at once  
- **Compatibility**: Foundation for ML libraries (TensorFlow, PyTorch)  

---

## Getting Started  
1. Open in [Google Colab](https://colab.research.google.com/drive/1FZ8dZ9Ik61Yf2VMVRTkWu787y61ZJHmj?usp=sharing) or the [Kaggle Version](https://www.kaggle.com/code/deniskipeles/numpy-basics-for-begginers)
2. Run cells sequentially  
3. Experiment with parameters in examples  

---
