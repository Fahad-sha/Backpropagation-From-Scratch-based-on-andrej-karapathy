## 🧮 Backpropagation (Inspired by Andrej Karpathy - Zero to Hero)

Backpropagation is the core algorithm used to train neural networks by efficiently computing gradients of the loss function with respect to the model parameters.

### 🚀 Core Steps

1. **Forward Pass:**  
   - Inputs are passed through the network.
   - Each layer applies linear transformations (weights & biases) and nonlinear activations.
   - The final output is compared to the target to compute the **loss**.

2. **Backward Pass (Backpropagation):**  
   - Gradients of the loss are propagated backwards through the network using the **chain rule**.
   - Each parameter receives its gradient, showing how much it contributed to the total error.

3. **Parameter Update:**  
   - Parameters are updated (e.g., via **Stochastic Gradient Descent (SGD)**) to minimize the loss:
     $$\[
     \theta := \theta - \eta \frac{\partial L}{\partial \theta}
     \]$$
   - This process iteratively improves the network’s predictions.

### 🧠 The Computational Graph View

- The entire neural network can be represented as a **computational graph**.
- Each node represents an operation (addition, multiplication, activation).
- Backpropagation walks backward through this graph, applying the chain rule at each node to compute gradients efficiently.
- This allows even deep networks to be trained with millions of parameters.

### 🎯 One-Line Intuition

> Backpropagation = chain rule applied systematically across the computational graph to compute gradients for all model parameters.

### 📺 Resources (Highly Recommended)

- [Neural Networks: Zero to Hero (Andrej Karpathy YouTube Series)](https://www.youtube.com/watch?v=VMj-3S1tku0)
- [Micrograd: A tiny scalar-valued autograd engine (Karpathy GitHub Repo)](https://github.com/karpathy/micrograd)
- [CS231n: Backpropagation and Computational Graphs](https://cs231n.github.io/optimization-2/)

---

> This project follows Karpathy's "Zero to Hero" philosophy of building neural networks from scratch to deeply understand how backpropagation works at the core.

