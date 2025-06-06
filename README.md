This project explores the use of transformer-based neural networks to predict pitch sequences in Major League Baseball (MLB) games. Leveraging pitch-level data from Statcast and other sources, the goal is to model pitcher behavior and generate accurate, context-aware predictions of the next pitch thrown.

# Project Summary:
This notebook implements a transformer architecture, inspired by advances in natural language processing, to predict the next pitch type in a baseball at-bat. The sequence of past pitches and game context (such as count, runners on base, score, etc.) are treated as a time-series input. The model attempts to learn the underlying patterns and strategies used by pitchers based on historical data.

# Features:
Transformer model implementation in PyTorch
Preprocessing of pitch-by-pitch data using pybaseball and custom engineering
Contextual encoding of features like pitch count, batter/pitcher handedness, and base state
Focus on sequence modeling, inspired by language modeling techniques
Early experimentation with multiple architectures and batching strategies

# Dependencies:
Python 3.10+
PyTorch
pandas
numpy
pybaseball
scikit-learn
matplotlib

# Known Issues & Notes:
Long runtime during model training.
May require GPU acceleration for efficient training.
Data fetching via pybaseball can be slow and should be cached where possible.

# Future Work:
Incorporate more features (e.g., pitcher fatigue, weather, batter history)
Expand to include attention visualizations
Compare against baseline models (e.g., LSTM, Markov Chains)
Deploy a web-based interface for interactive pitch prediction
