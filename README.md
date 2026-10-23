# Electrical Engineering Chatbot Using a Small Language Model (SLM)

## Project Overview

This project focuses on developing an Electrical Engineering Chatbot using a Small Language Model (SLM) implemented in COBNOX. The chatbot is designed to answer fundamental electrical engineering questions and provide simple explanations of electrical concepts, electronic components, and circuit principles.

The model follows a custom training workflow that includes data preparation, pre-training, tokenization, Supervised Fine-Tuning (SFT), and response testing.

The training dataset contains 41 electrical engineering question-and-answer entries covering topics such as voltage, current, resistance, Ohm's Law, electrical components, circuit laws, electrical power, Multisim, MATLAB, and electrical safety.

## Project Features

- Electrical engineering question-answering chatbot.
- Custom dataset containing 41 question-and-answer entries.
- Small Language Model (SLM) training.
- Pre-training and Supervised Fine-Tuning (SFT).
- Tokenization and text preprocessing.
- Experiments with different model layers and training steps.
- Model execution through the COBNOX compiler.
- Testing with fundamental electrical engineering questions.

## Technologies and Tools

- **Programming Language:** COBNOX
- **Model Type:** Small Language Model (SLM)
- **Training Methods:** Pre-training and SFT
- **Dataset:** Custom Electrical Engineering Corpus
- **Tokenizer:** Model-compatible tokenizer
- **Execution:** COBNOX Compiler

## Dataset Preparation

A custom corpus was prepared with 41 question-and-answer entries. The dataset covers:

- Electrical engineering fundamentals
- Voltage, current, and resistance
- Ohm's Law and electrical power
- Resistors, capacitors, inductors, diodes, and transistors
- Open, closed, and short circuits
- Series and parallel circuits
- Kirchhoff's Current Law and Voltage Law
- Transformers, generators, and electric motors
- Multimeters and circuit protection
- Multisim and MATLAB
- Electrical safety

Each entry combines a question with its corresponding answer in a consistent text format.

## Training Workflow

### 1. Data Preprocessing

The electrical engineering corpus is prepared in a consistent format for the model training pipeline.

### 2. Pre-training

The model is trained on the prepared electrical engineering dataset to learn domain-specific terminology and text patterns.

### 3. Tokenization

The text is converted into tokens using the tokenizer required by the model.

### 4. Supervised Fine-Tuning (SFT)

The model is fine-tuned using structured prompts and corresponding responses to improve its ability to answer electrical engineering questions.

### 5. Model Testing

The trained chatbot is tested using electrical engineering questions to examine the relevance and consistency of its generated answers.

## Model Configuration Experiments

Different model configurations were tested by varying the number of layers and training steps.

| Experiment | Number of Layers | Training Steps |
|---|---:|---:|
| Experiment 1 | 1 | 60 |
| Experiment 2 | 1 | 50 |
| Experiment 3 | 2 | 50 |
| Experiment 4 | 2 | 75 |
| Final Configuration | 2 | 55 |

### Final Model Configuration

- **Number of Layers:** 2
- **Training Steps:** 55

The experiments were conducted to explore different training configurations and observe their effect on chatbot responses.

## Training Results

The following loss values were recorded during training:

| Training Stage | Loss |
|---|---:|
| Pre-training Loss | 0.3304 |
| SFT Loss | 0.0094 |

These values represent the recorded training losses for the respective stages. Further evaluation on unseen questions would be needed to measure generalization and overall answer accuracy.

## AI Response Testing

The chatbot was tested with electrical engineering questions. The following responses were generated:

**Test 1: Ohm's Law**

Question: What is Ohm's Law?

AI Response: Ohm's Law states that voltage equals current multiplied by resistance: V = I × R.

**Test 2: Voltage**

Question: What is voltage?

AI Response: Voltage is the electrical potential difference between two points in a circuit.

**Test 3: Electric Current**

Question: What is electric current?

AI Response: Electric current is the flow of electric charge through a conductor.

**Test 4: Multisim**

Question: What is Multisim used for?

AI Response: Multisim is an electronic circuit simulation program used to design, analyze, and test circuits virtually.

These tests demonstrate that the chatbot can generate relevant responses to several fundamental electrical engineering questions.

## Project Objective

The objective is to develop a lightweight, domain-specific chatbot capable of answering basic electrical engineering questions using a custom-trained Small Language Model implemented in COBNOX.

## Future Improvements

- Expand the electrical engineering training dataset.
- Add more advanced electrical engineering concepts.
- Evaluate responses using a larger set of unseen questions.
- Experiment with additional model configurations.
- Improve response accuracy and consistency.

## Disclaimer

This project is an educational experiment in Small Language Model development for electrical engineering question answering. Its responses are intended for learning purposes and should not replace professional engineering advice or electrical safety procedures.
