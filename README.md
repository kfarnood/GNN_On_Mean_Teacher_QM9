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

While fully supervised models achieve ~0.01 Debye MAE using 110k labels, models restricted to 10k labels typically achieve ~0.15-0.20 Debye. My Semi-Supervised Mean Teacher currently achieves 0.87 Debye, outperforming traditional ML baselines (Random Forest ~1.2 D) and establishing a working proof-of-concept for consistency regularization on quantum chemical graphs.

Well as of this date (28 Nov) both Grok and DeepSeek insist that I have broke the world record . But this is something that I need to communicate with the university.



Mean Teacher consistency regularization
Custom Angle-Aware GNN
ArcSinh MSE loss
200 epochs, first run, no tuning

AI Help : Grok for analysing the output, Deepseek for debugging and analyzing the output. Chat gpt was useless (as expected ) . Gemini for logic check and debug

License
MIT
