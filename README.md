# Background
**Machine learning** is a branch of artificial intelligence where data is used to "learn" patterns and make predictions or inferences about new data (rather than using explicit rules). In simpler terms, a mathematical model is developed by finding patterns in training data. The model is "tuned" or "adjusted" for accuracy as more data become available. 

What is **Polynomial Regression**?
Polynomial regression is a technique used to model the relationship between a dependent variable (what you're trying to predict) and an independent variable (what you're basing your prediction on) when that relationship isn't straight line. Polynomial regressions are capable to fit curves by leveraging polynomial equations. 

y =β₀ + β₁x + β₂x² + β₃x³ + … + βₙxⁿ

**Deep learning** utilizes artificial *neural networks* with multiple layers, as opposed to the explicitly designed algorithms employed in traditional machine learning.

What is **Neural Network**?
A neural network is a machine learning model that uses interconnected "nodes" which are organized in layers and learns pattern-recognizing weights and biases from data to map inputs to outputs. *Weights* act like dials that control how strongly each input feature influences the decision. *Biases* are built-in values that shift the decision threshold, allowing a neuron to activate even if the inputs themselves are weak. Together, these model parameters determine how each node contributes to the overall computation.

<img width="650" height="254" alt="image" src="https://github.com/user-attachments/assets/b02d6474-70bf-43d6-92e5-6a420f6de60d" />

The power of a neural network comes from its ability to learn the right weights and biases from data. This is done by comparing the network’s prediction to the true output and measuring the error using a loss function. Overfitting is a common problem in all kinds of neural networks.
<p align="center">
<img width="400" height="254" alt="image" src="https://github.com/user-attachments/assets/988f8736-61df-4aeb-8a6e-e64c1969771e" />
</p>

# Physics-Informed Neural Networks
Creating numerical models of physical systems is important to simulate the system behavior without building physical prototypes, which can be time-consuming and expensive. While simplified physics models capture basic behavior, they don't represent the more complex dynamics, such as friction and resistance of the physical system. 

**Physics-Informed Neural Networks** (PINNs) use simplified physics equations as a foundation and apply deep learning to model the residual errors (due to complex/nonlinear characteristics) between these simplified models and actual observations. This hybrid approach combines the interpretability and generalizability of physics with the pattern-recognition power of neural networks, producing more accurate system representations without requiring massive amounts of data.
<p align="center">
<img width="560" height="237" alt="image" src="https://github.com/user-attachments/assets/ebc4d9d4-1656-412a-943a-87685b3c19aa" />
</p>

*Raissi, Perdikaris, and Karniadakis* introduced **Physics-Informed Neural Networks** where neural networks were explicitly trained to solve problems while complying with identifiable physics laws expressed as nonlinear PDEs. This is done by including the differential equations directly into the loss function when training the neural network.

Given the specific boundary conditions & initial conditions, <img width="129" height="58" alt="image" src="https://github.com/user-attachments/assets/6388a615-6f14-4aab-9608-e35c03a90959" /> has a solution 𝑢=𝑓(𝑥,𝑦,𝑡), 

<p align="center">
  <img width="553" height="356" alt="image" src="https://github.com/user-attachments/assets/5c724387-68ca-4597-b7af-6d518cb7bf29" />
</p>

# References
- https://www.ibm.com/think/topics/machine-learning
- https://www.mathworks.com/discovery/physics-informed-neural-networks.html
- https://i-systems.github.io/tutorial/KSNVE/220525/01_PINN.html
- https://benmoseley.blog/my-research/so-what-is-a-physics-informed-neural-network/
