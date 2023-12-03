
Project Title: Backdoor Detection in Neural Networks Using Pruning Defense

Description
This repository contains the implementation of a backdoor detection system for neural networks, specifically targeting BadNets trained on the YouTube Face dataset. The project involves the development of a modified neural network, referred to as GoodNet, capable of classifying both clean and backdoored inputs by introducing an additional classification category.

Environment
- MacBook Pro with M1 chip
- Jupyter Notebook

Contents
- Pruning_Defense.ipynb: The main Jupyter Notebook containing the implementation of the pruning defense and GoodNet.
- eval.py: A script for evaluating the model's performance on clean and backdoored data.
- Data/: Directory containing the validation set (valid.h5) and test set (test.h5).
- Models/: Directory where the original, pruned, and GoodNet models are saved.

Setup and Execution
1. Clone the repository to your local machine.
2. Ensure you have a Jupyter Notebook environment set up on a MacBook Pro with an M1 chip or a similar configuration.
3. Install necessary Python packages such as TensorFlow, Keras, etc., as listed in requirements.txt.
4. Navigate to the Data/ directory and ensure it contains the correct datasets.
5. Open Pruning_Defense.ipynb in Jupyter Notebook and execute the cells sequentially.
6. Use eval.py to evaluate the models. Ensure the path to the data and model directories in the script reflects your local setup.

Contributing
Contributions to this project are welcome. Please open an issue to discuss your ideas or submit a pull request with your changes.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
- Special thanks to the instructors and contributors of the CSAW-HackML-2020 for providing the dataset and initial guidance.
- Gratitude to NYU for the support and resources provided during the course of this study.
