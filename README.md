# DC-MAPO: Dual-Constrained Multi-Agent Policy Optimization

This repository contains the official implementation of **DC-MAPO**, a multi-agent reinforcement learning algorithm designed to enforce safety constraints in financial trading and cooperative navigation tasks.

## Key Results

**Transaction Cost Efficiency (Section III)**
DC-MAPO significantly reduces portfolio turnover while maintaining high returns, effectively solving the "churning" problem in high-frequency trading.

**Mechanism Activation (Section I)**
On the NASDAQ dataset, the method converges to a high-fidelity regime ($>0.84$) compared to unconstrained baselines ($0.20$).

## Code Organization

The experiments are split into three notebooks corresponding to the paper sections:

| Notebook | Paper Section | Description |
| :--- | :--- | :--- |
| **`notebooks/01_Train_NASDAQ.ipynb`** | **Section I** | Runs the core mechanism activation experiments on NASDAQ. Generates Learning Curves & Fidelity Distributions. |
| **`notebooks/02_Train_SP500.ipynb`** | **Section II** | Runs generalization experiments on S&P 500 data to test hyperparameter stability. |
| **`notebooks/03_Train_MPE_TC.ipynb`** | **Section III, V** | Runs the **Transaction Cost** analysis (Section III) and the **MPE Cooperative Navigation** boundary test (Section V). |

## 🚀 Usage

1. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
