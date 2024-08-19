# Deep Reinforcement Learning Stock Trading Project

This project uses deep reinforcement learning (DRL) to manage a stock trading portfolio. The agent makes trading decisions (buy, hold, sell) based on historical stock data and is rewarded based on net unrealized profits.

## Project Structure

- **train.py**: Script to train the DRL agent.
- **evaluate.py**: Script to evaluate the trained model.
- **requirements.txt**: List of dependencies.
- **logs/**: Directory for TensorBoard logs.
- **saved_models/**: Directory for saved models.
- **data/**: Directory for stock data used in training and evaluation.

## Getting Started

1. Install dependencies:
   ```bash
   pip3 install -r requirements.txt
   ```

2. Train the agent:
   ```bash
   python3 train.py --model_name=DQN --stock_name=^GSPC_2010-2015
   ```

3. Evaluate the agent:
   ```bash
   python3 evaluate.py --model_to_load=DQN_ep10 --stock_name=^GSPC_2018
   ```

4. Visualize training loss and portfolio value:
   ```bash
   tensorboard --logdir=logs/model_events
   ```
