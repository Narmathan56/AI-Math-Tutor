**AI Model Development**

For the early stage of this project, I chose a Transformer architecture because it is well suited for sequence-to-sequence tasks and complex reasoning problems. Since mathematical reasoning often involves step-by-step transformations, transformer models provide an effective structure for learning these patterns.

When I first started the project, I had very limited knowledge of deep learning. To build the necessary foundation, I studied machine learning concepts using resources from my university library and online learning platforms. One of the key learning resources was the Deep Learning Specialization by DeepLearning.AI, where I learned fundamental concepts including:

- Mathematical notation used in machine learning
-Gradient descent optimisation
- Logistic regression
- Derivatives and backpropagation
- Computation graphs
- Vectorisation techniques

In addition to these learning resources, I completed certification courses including:

- NVIDIA AI and Application Development
- Microsoft Azure AI-900

Using this knowledge, I gradually built the model architecture step by step. The model development included implementing core transformer components such as:

- Positional encoding
- Attention mask creation
- Transformer layers
- Training loops and optimisation processes

During the first five months of development, the model did not produce stable results. This period involved significant experimentation with different architectures, training strategies, and parameter configurations. Through continuous testing and iteration, the model eventually began to converge during training.

After tuning important parameters such as:

- number of attention heads
- number of layers
- training epochs

the model achieved the following training results:

- Final training loss: 0.365
- Accuracy: 0.9810

Reaching this stage was a major milestone in the development process and confirmed that the architecture was capable of learning mathematical patterns effectively.

**Dataset Collection**

The datasets used for training were collected from multiple sources, including:

- DeepMind Mathematics Dataset
- Kaggle mathematical datasets
- Custom datasets created using the Pandas framework

Although large datasets are available, the initial training experiments used approximately 1000 samples. When attempting to train the model with significantly larger datasets (200,000+ examples), additional challenges appeared, including the need for further architecture tuning and greater computational resources.

To address this issue, a progressive training strategy was adopted:

- Start with smaller datasets
- Validate the architecture and training behaviour
- Gradually scale to larger datasets once the system becomes stable

This approach allows faster experimentation while reducing computational requirements during early development.

**Visualisations and Interactive Charts**

Interactive charts and visualisation tools are also being developed to analyse both student learning behaviour and model performance.

These visual systems will support:

- educational feedback for students
- analysis of learning progress
- early marketing research and user behaviour insights

Understanding how students interact with the tutoring system will help improve the explanation quality and identify areas where additional support is needed.

**Transition to Current Development Approach**

Although the custom transformer model achieved promising results, building a full reasoning system entirely from scratch would significantly slow down product development. Since one of the key goals of this project is to deliver a functional tutoring platform as quickly as possible, a strategic decision was made to change the system architecture.

The project is now moving toward a hybrid AI approach, where pre-trained large language models are used for complex reasoning and explanation generation, while the custom transformer model functions as a specialised deterministic prediction component inside the system.

This strategy allows faster product shipping, better reasoning performance, and a more scalable system architecture while still preserving the research work done during the early stages of development. 


# 🧠 AI Math Tutor System

---

## 📌 Current Development Status

Hello, I am **Narmathan**, the developer of the AI Math Tutor project.

At the current stage, I have successfully built an initial chatbot interface using the **Gemini model**. This chatbot can respond to mathematical queries and generate explanations.

However, the long-term vision is much bigger than a chatbot. The system is being developed into an **adaptive AI teacher** that can:

- 🧠 Understand student thinking
- ❌ Detect mistakes
- 🔍 Identify misconceptions
- 📊 Provide guided step-by-step learning
- 🖊️ Use an interactive whiteboard for teaching

---

## 🏗️ Planned Adaptive Tutoring Pipeline

The system follows a structured reasoning pipeline:

Student Input
↓
Step Parser (Gemini extraction)
↓
Validation Checker
↓
Error / Misconception Classifier
↓
Misconception Knowledge Database Lookup
↓
Explanation Generator
↓
Decision Router
↓
Output (Text + Speech + Whiteboard Animation)







💡 This design ensures the system focuses on **reasoning process**, not just final answers.

---

## ✍️ Step Parser

The Step Parser acts as a bridge between human language and machine reasoning.

### 🔹 Responsibilities:

- 📥 Reads full student input
- ✂️ Splits solution into logical mathematical steps
- ➗ Identifies expressions and operations
- 🧾 Converts reasoning into structured format
- 📤 Sends structured data to error analysis system

💡 Purpose: Convert natural language into analyzable mathematical structure.

---

## ✔️ Validation Checker (SymPy)

The system uses **SymPy (symbolic mathematics library)** for validation.

### 🔹 Functions:

- ✔️ Checks correctness of mathematical steps
- 🔢 Validates transformations
- 🧠 Ensures reliable AI feedback
- ⚙️ Acts as a mathematical truth layer

💡 This module guarantees **mathematical accuracy before explanation is shown**.

---

## 🧠 Hybrid AI Model Architecture

The system uses a hybrid multi-model design:

### ⚡ Custom Transformer Model
- Fast arithmetic predictions
- One-digit operations (addition, multiplication)
- Lightweight computation tasks

### 🧩 Gemini Model
- Deep reasoning engine
- Step-by-step explanations
- Complex problem solving

### 💬 Llama Model
- Surface-level reasoning
- Quick conversational responses

💡 Each model is used based on task complexity.

---

## 🎯 Decision Router

The Decision Router selects the best model for each task.

### 🔹 Routing Logic:

- ⚡ Simple arithmetic → Transformer Model
- 🧠 Complex reasoning → Gemini 2.5 Flash
- 💬 Quick responses → Llama Model

### 🔹 Benefits:

- 🚀 Faster response time
- 🧠 Better reasoning quality
- ⚙️ Efficient system performance

---

## ⚠️ Development Challenges

During early development:

### 🔧 Technical Issues:

- FastAPI server setup (port 8000)
- Gemini service on Colab (port 8001)
- Cross-service communication failures

### ❌ Problems Faced:

- HTTP 403 security errors
- API connection instability
- Backend integration breakdown

💡 Key Learning:
> System architecture and security are just as important as AI models.

---

## 🔄 Strategy Change (Architecture Upgrade)

The development approach has been upgraded:

👉 From manual integration  
👉 To **LangGraph + LangChain orchestration**

### 🔹 Why this change:

- 🔗 Easier multi-model coordination
- ⚙️ Faster development cycle
- 🧩 Modular architecture
- 🚀 Scalable AI pipeline design

💡 This allows focus to shift from backend issues to **core product innovation**.

---

## 🛣️ Updated MVP Development Plan

The MVP is structured into **4 phases**:

---

## 🧱 Phase 1 — Core Reasoning Engine

- 🧠 LangGraph orchestration system
- 🧩 Gemini + Llama integration
- ✍️ Step Parser implementation
- ✔️ SymPy validation system

---

## 🧠 Phase 2 — Pedagogical Intelligence

- ❌ Misconception detection engine
- 📊 Learning memory system
- 🖊️ Basic whiteboard interface
- 🎯 Personalized feedback system

---

## 🎨 Phase 3 — Interactive Learning System

- ✏️ Animated step-by-step explanations
- ⚡ Real-time tutoring responses
- 🧪 System testing and optimization
- 📈 Accuracy improvements

---

## 🚀 Phase 4 — MVP Launch

- 🎨 UI/UX refinement
- 🧪 User testing with students
- ⚙️ Performance improvements
- 🌍 Early deployment preparation

---

## 🎯 Vision

The goal is to build an **AI tutor that thinks like a teacher**, not just a chatbot.

A system that can:

- 🧠 Understand student thinking
- ❌ Detect misconceptions
- ✍️ Explain clearly step-by-step
- 📈 Adapt to each learner

---

## 💡 Final Goal

This is not just an AI system.

It is a **personalised learning intelligence platform** designed to replicate how real teachers guide students.

---

