# HW2: Policy-Based Reinforcement Learning Algorithms

This repository hosts an implementation of two key policy-based reinforcement learning algorithms: Vanilla Policy Gradient (REINFORCE) and Policy Gradient with Baseline, fundamental in Deep Reinforcement Learning (RL). REINFORCE, a classic policy-based method, adjusts policy parameters using the expected reward's gradient, training a neural network to maximize rewards in RL environments. The Policy Gradient with Baseline extends this by incorporating a state-value function as a baseline, reducing gradient variance and enhancing learning stability.

These algorithms are tested in the Ant-v4 environment from Gymnasium, which simulates a four-legged robot in a complex environment with a continuous action space. This setup demands refined strategies for action selection and policy development, demonstrating the algorithms' effectiveness in handling sophisticated, real-world scenarios. The repository serves as a practical demonstration of advanced policy optimization techniques in RL, showcasing end-to-end training and effective handling of continuous action spaces.

## Repository Contents

- `hw2_F.ipynb`: I-Python Notebook containing the implementation of  Vanilla Policy Gradient (REINFORCE) and Policy Gradient with Baseline algorithms, along with the code for running experiments in the Ant-v4 environment.
- `hw2_F.py`: A Python script with the core logic for the reinforcement learning algorithms, which can be imported and used in other projects or scripts.
- `hw2_F-ipython.pdf`: A PDF export of the I-Python Notebook, which includes all the code, outputs, and visualizations for those who prefer to read without execution.
- `README.md`: This file, providing an overview and instructions for the repository.
- `Report - HW2.pdf`: A detailed report of Question 2 and Question 3 results of the experiments, visual plots, theoretical explaination and analysis of the performance of the algorithms.


## Getting Started

* Follow these instructions to set up the environment and run the algorithms on google colab.

### Prerequisites

* Before running the notebook, ensure that you have Python (version 3.x) installed on your machine and the following package:

```
pip install gymnasium[mujoco]
```

### Installation
* Download the "hw2_F.ipynb" file directly.
* Open the notebook in Jupyter Notebook or Google Colab.
* Execute the command provided above to install the necessary package.
* Run all cells in the notebook to see the algorithms in action.

### Running the Notebook

# If using Jupyter Notebook
jupyter notebook hw2_F.ipynb

# If using Google Colab (Preferred)
Upload the notebook to your Google Colab session and run it there.

* For "PG Algorithm Output", or "PGB Algorithm Output", simulate command-line argument by  replace 'pg' with 'pgb' to run policy gradient with baseline as follows.
* For Vanilla Policy Gradient:
    ```
        sys.argv = ['hw2_F.py', '--algo', 'pg']
        # Then call the main function
        if __name__ == '__main__':
            main()
    ```
* For Policy Gradient with Baseline:
    ```
        sys.argv = ['hw2_F.py', '--algo', 'pgb']
        # Then call the main function
        if __name__ == '__main__':
            main()
    ```