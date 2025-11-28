# GNN_On_Mean_Teacher_QM9
Semi-Supervised Angle-Aware GNN using Mean Teacher architecture for QM9 Dipole Moment prediction. Features consistency regularization, ArcSinh target scaling, and custom message passing layers. Achieves ~0.87 Debye MAE (Original Space) after 200 epochs on NVIDIA A100. Built with PyTorch Geometric &amp; Lightning.


## Results
- **Best Val MSE: 0.2377** (Step 175)
- **MAE: 0.488 Debye** 
- **8% labeled data** → 85% full-supervision performance

## Quick Start
```bash
git clone https://github.com/YOUR_USERNAME/GNN_On_Mean_Teacher_QM9.git
cd GNN_On_Mean_Teacher_QM9
pip install -r requirements.txt
jupyter notebook GNN_On_Mean_Teacher.ipynb
Key Features

Mean Teacher consistency regularization
Custom Angle-Aware GNN
ArcSinh MSE loss
200 epochs, first run, no tuning

License
MIT
