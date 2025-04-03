# 🔋 Battery Temperature Prediction Using Deep Learning and Transformers

This repository contains the implementation and analysis of deep learning models for accurate **temperature prediction of Panasonic 18650PF Lithium-Ion cells**, based on **Electrochemical Impedance Spectroscopy (EIS)** data collected at varying ambient temperatures.

## 📘 Abstract

Maintaining the **safety**, **longevity**, and **performance** of lithium-ion cells is critical for high-demand applications such as **electric vehicles** and **energy storage systems**. This study explores deep learning techniques—especially **Transformers** and **Recurrent Neural Networks (RNNs)**—to predict battery temperature from EIS data.

The models evaluated include:
- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Bidirectional LSTM (Bi-LSTM)
- Minimal Gated Unit (MGU)
- Transformer-based architectures

The study concludes that while **GRU** performs best individually, **ensemble approaches** offer the most efficient trade-off between speed and accuracy.

## 📊 Results

| Model        | MSE    | RMSE   | R² Score |
|--------------|--------|--------|----------|
| LSTM         | 1.4996 | 1.2246 | 0.9943   |
| GRU          | **0.9615** | **0.9806** | **0.9963**   |
| Bi-LSTM      | 1.0734 | 1.0360 | 0.9959   |
| Ensemble     | 1.1535 | 1.0740 | 0.9956   |

> ✅ **GRU** achieves the best performance across all metrics.  
> 🔄 **Ensemble models** still offer a good balance between performance and generalization.  
> 🔍 While **LSTM and Bi-LSTM** perform decently, they trail slightly behind GRU and ensemble methods.

## 🧠 Models & Techniques

- 📈 **Data Source**: Electrochemical Impedance Spectroscopy (EIS)
- 🧠 **Models**:
  - LSTM
  - GRU
  - Bi-LSTM
  - MGU
  - Transformer
- 📏 **Metrics**:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score
