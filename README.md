# Programming for AI (Part II)

Official repository for the second part of the 2026 edition of the **Programming for AI** course, integrated into the Specialization Degree: [**"Applied Artificial Intelligence and its Mathematical Foundations"**](https://www.ehu.eus/en/web/graduondokoak/university-specialisation-applied-artificial-intelligence-mathematical-foundations) at the University of the Basque Country (UPV/EHU).

---

## 🎯 Objectives

The primary goal of this course is to bridge the gap between theoretical mathematical foundations and practical implementation. Students will:
- **Master Advanced Toolsets:** Gain proficiency in the latest high-performance programming frameworks (specifically JAX and Keras/TensorFlow).
- **Understand Low-Level Abstractions:** Deconstruct how Neural Networks operate under the hood, from tensor operations to functional programming paradigms.
- **Develop End-to-End Pipelines:** Learn to handle the full lifecycle of an AI model, from raw data ingestion and "leakage-free" splitting to custom training loops.
- **Bridge Theory and Code:** Translate mathematical concepts, such as automatic differentiation ($ \nabla f $) and optimization algorithms, into efficient, vectorized code.

---

## 🛠 Lessons Dynamics & Methodology

This course follows a **tutorial-oriented practical approach**. Rather than traditional lectures, the dynamics are designed as follows:

### The Material
All teaching materials consist of **self-explained Jupyter Notebooks**. These documents contain:
- Theoretical context and code explanations.
- Guided implementation examples.
- 📋 **Embedded Exercises:** Specific tasks that must be addressed *during the lesson* hours.

### Classroom Flow
1. **Guided Navigation:** We will progress through the notebooks together.
2. **Active Coding:** When we reach an exercise, students will be given a dedicated time slot to solve it.
3. **Common Discussion:** After the coding time, we will hold a collective discussion to analyze different solutions, difficulties, etc..

### Grading & Submission
The Jupyter Notebooks serve as the primary instrument for evaluation.
- **Mandatory Submission:** At the end of **each lesson**, students must send the `.ipynb` file in its current state (including the solutions to the exercises addressed that day) to the instructor via email/e-gela.

---

## 📅 Schedule

### Session 1: Neural Network Programming
- **Key Concepts:** Abstractions, APIs, and low-level components. Standard Keras pipeline.
- **Practice:** Basic examples using Keras for classification/regression handling different data types (features, images, time series). Model assessment and relevance of feature engineering.

### Session 2: DL Frameworks - JAX
- **Key Concepts:** Comparative analysis between TensorFlow, PyTorch, and JAX. Introduction to functional programming in AI.
- **Practice:** JAX fundamentals: Autodiff ($ \frac{\partial y}{\partial x} $), JIT compilation, and vectorization (`vmap`). Optimization with Optax.

### Session 3: Advanced JAX Programming
- **Key Concepts:** Advanced techniques to make code "JIT-able" and achieve maximum computing performance.
- **Practice:** Advanced `jit`, `vmap` and automatic differentiation in JAX.

### Session 4: Building a Model from Scratch (I)
- **Key Concepts:** Data lifecycle: capture, cleaning, and feature extraction. The importance of the i.i.d. (independent and identically distributed) assumption.
- **Practice:** Preparing ECG time-series signals. Implementing robust data splitting to avoid data leakage.

### Session 5: Building a Model from Scratch (II)
- **Key Concepts:** Design of experimental validation. Defining the optimization problem: Loss functions $ L(\theta) $, metrics, and hyperparameters.
- **Practice:** Building and validating models for the problem defined in Session 4. Overfitting assessment.

### Session 6: Customizing Keras
- **Key Concepts:** Keras tuning with JAX. Progressive disclosure of complexity.
- **Practice:** 
    - Creating custom Layers, Metrics, and Losses.
    - Overriding `train_step()` and `compute_loss_and_updates()`.
    - Advanced Callbacks and data-oriented interfaces.

### Session 7: Leveraging Existing Models
- **Key Concepts:** Integration of foundational models (LLMs) into custom pipelines.
- **Practice:** 
    - Local LLM deployment and programmatic querying.
    - Tokenizers and Embeddings.
    - Transfer Learning and Fine-tuning in Keras.
