CS50's Introduction to Artificial Intelligence with Python

Learning log for Harvard's CS50 AI (Harvard / edX), completed in November 2026 with the free CS50 certificate.

Note: in line with CS50's academic honesty policy, the source code of my solutions is not published here. This repository only documents what I learned, the techniques used in each project, and the results obtained. Code can be shared privately on request.
	•	Certificate: [add link to your certificate here]
	•	Course: 7 weeks, 12 projects, all submitted and validated (check50 / style50)
	•	Stack: Python, NumPy, TensorFlow / Keras, scikit-learn, NLTK, Hugging Face Transformers

Overview

Week	Topic	Projects	Core techniques
0	Search	Degrees, Tic-Tac-Toe	BFS, minimax
1	Knowledge	Knights, Minesweeper	Propositional logic, model checking, inference
2	Uncertainty	PageRank, Heredity	Markov chains, Bayesian networks, sampling
3	Optimization	Crossword	CSP, arc consistency (AC-3), backtracking search
4	Learning	Shopping, Nim	k-nearest neighbors, Q-learning
5	Neural Networks	Traffic	Convolutional neural networks
6	Language	Parser, Attention	Context-free grammars, Transformers / attention

Week 0: Search

Concepts: state spaces, uninformed and adversarial search, depth-first and breadth-first search, minimax.

	•	Degrees: finds the shortest connection between two actors through the movies they appeared in, modeled as a graph and solved with breadth-first search.
	•	Tic-Tac-Toe: an unbeatable player built with the minimax algorithm.

Week 1: Knowledge

Concepts: propositional logic, entailment, inference by model checking, knowledge-based agents.

	•	Knights: solves "knights and knaves" logic puzzles by encoding each statement as a logical sentence and letting model checking deduce who is who.
	•	Minesweeper: an AI that plays Minesweeper by maintaining a knowledge base of sentences about mine locations and inferring safe moves and mines.

Week 2: Uncertainty

Concepts: probability, conditional probability, Bayesian networks, Markov models, approximate inference by sampling.

	•	PageRank: computes page ranks of a small web corpus in two ways: by sampling from a random-surfer Markov chain and by iterating the PageRank formula until convergence. Both approaches give consistent results.
	•	Heredity: a Bayesian network that computes the probability that each person in a family carries a gene or exhibits a trait, given partial evidence.

Week 3: Optimization

Concepts: constraint satisfaction problems (CSP), node and arc consistency, backtracking search, heuristics.

	•	Crossword: generates crossword puzzles as a CSP, using node consistency, the AC-3 algorithm and backtracking search with variable-ordering heuristics. check50: 24/25.

Week 4: Learning

Concepts: supervised learning, k-nearest neighbors, evaluation metrics (sensitivity / specificity), reinforcement learning, Q-learning.

	•	Shopping: a k-nearest-neighbors classifier that predicts whether an online shopping session ends in a purchase, evaluated with sensitivity and specificity.
	•	Nim: an AI that teaches itself to play Nim by playing against itself with Q-learning, then plays against humans.

Week 5: Neural Networks

Concepts: neural networks, backpropagation, overfitting and regularization (dropout), convolutional networks, TensorFlow / Keras.

	•	Traffic: a convolutional neural network that classifies traffic sign images from the GTSRB dataset (43 categories). Test accuracy: 96.92%.

Week 6: Language

Concepts: syntax and semantics, context-free grammars, n-grams, word embeddings, attention and Transformers.

	•	Parser: a context-free grammar plus a parser that extracts noun phrase chunks from English sentences, using NLTK.
	•	Attention: probes a pretrained masked language model (BERT) to visualize attention heads and analyze what linguistic relations they capture.

Key takeaways

	•	Search, logic and probabilistic reasoning remain the foundation behind many "classical" AI systems.
	•	Many problems reduce to the same core idea: model the problem formally (graph, CSP, Bayesian network), then apply the right algorithm.
	•	Moving from classical methods to learned ones (k-NN, Q-learning, CNNs, Transformers) shows the trade-offs between interpretability, data requirements and performance.

Next steps

	•	Build a personal AI project from scratch (to be published in a separate repository).
	•	Go deeper into machine learning theory and deep learning.