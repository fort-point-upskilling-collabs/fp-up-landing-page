# Fort Point Upskilling Collaboration Project Catalog — Long Edition

Detailed project menu for choosing a GitHub collaboration or learning project. Each entry includes its maturity, working location, purpose, and likely tools; the companion Short Edition is designed for faster browsing.

### Pocket Cocktail Party
**Repository:** https://github.com/bballdave025/pocket-cocktail-party  
**Status:** Prototype / active experiment  
**What It Is:** Blind-source-separation project that starts with understandable synthetic mixtures and Independent Component Analysis, then moves toward messier real recordings. It keeps the mixing geometry visible instead of treating audio separation as a black box.  
**Tools and Concepts Used:** Python; ICA/BSS, linear algebra, signal processing, synthetic data, experimental design.

### Bilingual Boundary Lab
**Repository:** https://github.com/bballdave025/bilingual-boundary-lab  
**Status:** Prototype / active experiment  
**What It Is:** Uses only *War and Peace* to test how models from n-grams upward learn boundaries between Russian and embedded French. Extensions can compare explicit boundary tokens with weaker or implicit language-switch signals.  
**Tools and Concepts Used:** Python; n-grams, multilingual NLP, tokenization, sequence modeling, visualization.

### English Gorf
**Repository:** https://github.com/bballdave025/english-gorf  
**Status:** Prototype with an inconclusive first experiment  
**What It Is:** Tests whether English's Germanic and French history leaves detectable differences in letter-frequency distributions, initially comparing shorter and longer words. A collaborator could vary vocabulary size, similarity measures, visualization, or source-separation approaches.  
**Tools and Concepts Used:** Python; frequency vectors, cosine similarity, dictionaries/corpora, visualization, computational linguistics.

### Envelope ZIP Reading
**Repository:** https://github.com/bballdave025/envelope-zip-reading  
**Status:** Scaffold / collaboration-ready  
**What It Is:** MNIST digit-recognition project inspired by Michael Nielsen's online neural-network text. A good small collaboration would implement the simple hidden-layer model and CNN, then inspect individual mistakes rather than stopping at aggregate accuracy.  
**Tools and Concepts Used:** Python; neural networks, CNNs, MNIST, classification, error analysis, linear algebra.

### JabberVec-l2v (X2vec family)
**Repository:** https://github.com/bballdave025/jabbervec-l2v  
**Status:** Prototype / active experiment  
**What It Is:** Character-level modeling experiment asking what geometry learned letter embeddings develop from English-like text. It is intentionally small enough to inspect embeddings, generation behavior, and low-rank structure directly.  
**Tools and Concepts Used:** Python/PyTorch; embeddings, PCA/SVD, character models, low-rank approximation, visualization.

### Latent Forge
**Repository:** https://github.com/bballdave025/latent-forge  
**Status:** Active experiment  
**What It Is:** Small recommender-system laboratory built around simple baselines, matrix factorization, and holdout MSE. The emphasis is on changing one assumption at a time and justifying added complexity.  
**Tools and Concepts Used:** Python; recommender systems, matrix factorization, low-rank models, linear algebra, evaluation.

### Text Cleanroom
**Repository:** https://github.com/bballdave025/text-cleanroom  
**Status:** Active tooling project  
**What It Is:** Deterministic toolkit for finding and repairing messy text and filename encodings while keeping changes auditable.  
**Tools and Concepts Used:** Python; Unicode/encoding, CLI design, preprocessing, data quality, testing.

### Multimodal Jupy Logger
**Repository:** https://github.com/bballdave025/multimodal-jupy-logger  
**Status:** Experimental tooling  
**What It Is:** Captures Jupyter/IPython work as durable multimodal logs that can later be replayed or rendered, emphasizing experiment provenance rather than only notebook state.  
**Tools and Concepts Used:** Python/Jupyter; MIME handling, event logging, provenance, reproducibility.

### Mendeleev Spelling Bee
**Repository:** https://github.com/bballdave025/mendeleev-spelling-bee  
**Status:** Working prototype  
**What It Is:** Multilingual word game that tests whether words can be represented as sequences of chemical-element symbols, extending beyond English into Cyrillic and other scripts. Possible extensions include printable designs and experiments with symbol systems beyond ordinary alphabets.  
**Tools and Concepts Used:** Python; Unicode, tokenization, search/segmentation, CLI design, pytest/TDD.

### Start Pirate Now
**Repository:** https://github.com/bballdave025/start-pirate-now  
**Status:** Small learning experiment  
**What It Is:** Began as R interview preparation—the pirate pun is “Arrr!”—by systematically working through the language's built-in help and command-line documentation. The same approach can be reused to learn another compact tool or language from its canonical documentation.  
**Tools and Concepts Used:** R; documentation-driven learning, scripting, basic data structures.

### Double-P Double-N
#### Paper/Pencil Neural Networks
**Repository:** https://github.com/bballdave025/double-p-double-n  
**Status:** Minimal prototype / larger research seed  
**What It Is:** First small implementation of the Paper/Pencil Neural Networks idea: physically inspectable neural networks that can scale from pedagogy toward questions about computational and representational cost.  
**Tools and Concepts Used:** Neural networks, linear algebra, computational complexity, information theory, hands-on visualization.

### Discrete Fourier Transforms and Sampling
**Repository:** https://github.com/bballdave025/discrete_fourier_transforms_and_sampling  
**Status:** Small teaching/scientific-computing project  
**What It Is:** Short Mathematica-based introduction to Fourier analysis and sampling originally used to explain concepts relevant to ASR work. It could be recreated in Python or expanded into a signal-processing project.  
**Tools and Concepts Used:** Wolfram Language/Mathematica; DFT/FFT, sampling, signal processing, computational mathematics. Computer language crossover.

### Higgs Boson Visualized
**Repository:** https://github.com/bballdave025/higgs_boson_visualized  
**Status:** Scientific-visualization project  
**What It Is:** Particle-physics visualization work centered on Higgs-boson concepts, suitable as a starting point for reproducible quantitative physics communication.  
**Tools and Concepts Used:** Scientific computing/visualization; particle physics, quantitative plotting.

### RWKV + LoRA Learning Experiment
**Repositories:** https://github.com/bballdave025/rwkv-lora and https://github.com/bballdave025/info-rwkv-lora-learning-ref  
**Status:** Experimental / ambiguous result  
**What It Is:** Attempted LoRA fine-tuning work on RWKV, with supporting learning/reference material. The experiment produced behavior worth reconstructing rather than being presented as a clean success.  
**Tools and Concepts Used:** Python; RWKV, LoRA/PEFT, sequence models, loss curves, training diagnostics.

### Job Application Word Frequency
**Repository:** https://github.com/bballdave025/job-app-word-freq  
**Status:** Small text-analysis tool  
**What It Is:** Compares language in job descriptions and application materials using lightweight frequency analysis.  
**Tools and Concepts Used:** Python; tokenization, word frequencies, text comparison, visualization.

### Cyrillic-through-Latin OCR
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / dataset-building experiment  
**What It Is:** Build paired data by copy/pasting true Cyrillic text while separately using Android/Pixel screen-selection OCR to capture its Latin-biased corruption. The resulting pairs could train a model to reverse similar historical OCR errors.  
**Tools and Concepts Used:** Mobile data collection; OCR, Unicode/Cyrillic, sequence transduction, noisy-channel modeling.

### Multilingual Name Corruption Lab
**Repository:** Not yet created  
**Status:** Idea / larger family-history experiment  
**What It Is:** Simulate historical forms and mistakes for one surname, initially `KIMONT`, across languages, declensions, clerk transcription, typing, OCR, and eventually ASR. The goal is to generate better search variants for transformed historical names.  
**Tools and Concepts Used:** Python/LLMs; synthetic data, transliteration, morphology, OCR/ASR error models, multilingual NLP.

### DIAL / Digital Sundial Learning
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / scalable experiment  
**What It Is:** Learn the mapping needed for a digital sundial, starting with only 3 bits and seven hour states, then increasing resolution toward finer time intervals and more realistic geometry.  
**Tools and Concepts Used:** Python; binary representation, function approximation, geometry, optimization, model complexity.

### MorphoGender (X2vec family)
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / collaboration-ready small experiment  
**What It Is:** Test how well models can predict grammatical gender from the written forms of Russian and French nouns, asking how much supposedly memorized gender is encoded in morphology and etymological patterns.  
**Tools and Concepts Used:** Python; classification, feature engineering, morphology, interpretable ML, NLP.

### Syntactic Case Marking and Adpositions (X2vec family)
**Repository:** Not yet created  
**Status:** Idea / collaboration-ready larger experiment  
**What It Is:** Test how well models can predict the adposition or inflection that marks a noun phrase's relationship to the rest of a sentence. The project can compare language types and also examine non-adpositional functions of grammatical cases—a larger counterpart to MorphoGender.  
**Tools and Concepts Used:** Python and NLP toolkits; POS tagging, classification, feature engineering, morphology, interpretable ML.

### Ambiguity Corpus
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / larger research seed  
**What It Is:** Build a corpus of naturally occurring and constructed ambiguities using clarification phrases, syntactic ambiguity, puns, and minimal examples. It could support ambiguity classification and tests of whether LLMs can identify and justify multiple readings. Could easily loan elements to and borrow elements from the Measuring Instruction Inconsistency project.  
**Tools and Concepts Used:** Python/regex/LLMs; corpus construction, parsing, ambiguity taxonomy, NLP evaluation.

### Measuring Instruction Inconsistency
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea  
**What It Is:** Develop quantitative ways to detect when instructions or requirements conflict with one another, especially in LLM-facing tasks. Involves experiment design. Could easily loan elements to and borrow elements from the Ambiguity Corpus project.  
**Tools and Concepts Used:** Python/LLMs; evaluation metrics, constraint consistency, NLP, experimental design.

### Twain/Feynman Model Collapse
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / staged experiment  
**What It Is:** Begin with playful Twain↔Feynman style transformations: how might Richard Feynman tell a Mark Twain story, or Twain reshape a Feynman lecture? The research phase then studies what happens when a model is repeatedly trained on generated output from itself or another model.  
**Tools and Concepts Used:** Python/LLMs; style transfer, synthetic data, language modeling, constrained language generation, evaluation, humor in research, model-collapse experiments.

### Mechanics: Lagrange / Hamilton / T−V Simulations
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / computational-physics project  
**What It Is:** Build small simulations that compare different formulations of classical mechanics and make their mathematical relationships visible computationally.  
**Tools and Concepts Used:** Python; classical mechanics, ODEs, numerical methods, Lagrangian/Hamiltonian formulations.

### RLHF Incomplete Ontology
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea  
**What It Is:** Explore what happens when annotation or preference-learning tasks force judgments through an ontology that cannot represent all relevant cases.  
**Tools and Concepts Used:** RLHF, annotation design, ontology modeling, classification, evaluation.

### Design by Inverse Angular Light
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / vision-stage  
**What It Is:** Optics/geometry-oriented design idea centered on reasoning backward from angular light behavior to a desired physical configuration.  
**Tools and Concepts Used:** Geometry, optics, inverse problems, computational modeling.

### Info Theory for Pareidolia/Apophenia
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / academic-paper seed  
**What It Is:** Asks whether functional-information ideas can measure text-like or manuscript-like structure independently of OCR or handwritten-text-recognition results, including cases where people or models perceive meaningful patterns in noise.  
**Tools and Concepts Used:** Information theory, visual perception, image analysis, experimental design, digital humanities.

### NLP-Oriented Symbolic Encodings for Visual Structure
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / vision-stage  
**What It Is:** Explore ways to encode visual structure symbolically so methods normally associated with language models can operate on spatial or visual relationships.  
**Tools and Concepts Used:** Computer vision, symbolic representations, NLP, sequence modeling.

### Symbolized Persistence Under Quantized Projection
**Repository:** https://github.com/bballdave025/dwb-ip-notes  
**Status:** Idea / vision-stage  
**What It Is:** Study which symbolic or structural information survives quantization or projection into lower-detail representations.  
**Tools and Concepts Used:** Quantization, information theory, representation learning, dimensionality reduction.

### Underground Systems Prediction Dataset
**Repository:** Not yet created  
**Status:** Idea / multi-person collaboration candidate  
**What It Is:** Build a worldwide dataset of metros, subways, undergrounds, and tube systems using construction, geology, engineering, expansion, accident, and remediation features, then test which properties or outcomes can be predicted from the others.  
**Tools and Concepts Used:** Python/R; dataset design, regression/classification, feature engineering, correlation analysis, validation.

## Author-Attribution Project Family

These related projects examine which aspects of writing style survive changes in time, language, translation, model, or prompt.

### Style Trajectories
**Repository:** Not yet created  
**Status:** Idea / collaboration-ready NLP project  
**What It Is:** Tests whether models treat an author's early and late works as the work of one writer, and which stylistic signals remain stable or drift over a career.  
**Tools and Concepts Used:** Python; authorship attribution, stylometry, temporal analysis, NLP, corpus design.

### Translated-Author Attribution Experiment
**Repository:** Not yet created  
**Status:** Idea / collaboration-ready NLP project  
**What It Is:** Train models to distinguish two authors in their original language, then measure how author-identification confidence changes across translations. A stronger variant translates authors from different languages into each other's language and tests which stylistic signals survive.  
**Tools and Concepts Used:** Python; authorship attribution, stylometry, translation, NLP, cross-lingual evaluation.

### LLM Author Attribution Analysis
**Repository:** Not yet created  
**Status:** Idea / collaboration-ready LLM research project  
**What It Is:** Uses authorship-attribution methods to test how distinguishable open-ended responses are across language models, model configurations, prompts, and repeated runs. Controlled generation makes it possible to compare both inter-model and within-model stylistic diversity.  
**Tools and Concepts Used:** Python, command-line interfaces to LLMs; authorship attribution, stylometry, NLP, cross-model evaluation.

### Relating Hip Hop/Rap to Germanic and Skaldic Poetry (X2vec family)
**Repository:** Not yet created  
**Status:** Developed idea with experimental plans  
**What It Is:** Compare alliteration, internal rhyme, and repeated sound patterns in French and American hip-hop with Germanic and especially skaldic poetry. First let an unsupervised model discover patterns in open poetry corpora, then compare its findings with known poetic structures and, if useful, provide examples for guided learning.  
**Tools and Concepts Used:** Python; vectorization, clustering, unsupervised learning, sound-pattern analysis, comparative literature, NLP.

## More Mature Projects — On an Active Path to Publication

### CVMSS Research and Ontology Planning
**Repository:** Not publicly listed in this catalog  
**Status:** Published early phase / active research lineage  
**What It Is:** Uses computer vision to find reused manuscript fragments in historical book bindings, while supporting later work in dataset design, classification ontology, provenance, high-resolution modeling, explainability, and experiment design.  
**Tools and Concepts Used:** Python/Jupyter; computer vision, transfer learning, ResNet-50, Grad-CAM, dataset curation, provenance, manuscript studies.

### CVMSS Paper Code Prep
**Repository:** Not publicly listed in this catalog  
**Status:** Working experiment infrastructure  
**What It Is:** Cross-platform scaffold for reproducible paper and model experiments, including notebook creation, logging, testing, small proving experiments, and cloud-computing preparation.  
**Tools and Concepts Used:** Bash, PowerShell, Python/Jupyter; CIFAR-10, experiment scaffolding, testing, reproducibility, AWS/SageMaker.

## Abbreviation and Specialized-Term Guide

- **AI** — Artificial Intelligence
- **ASR** — Automatic Speech Recognition
- **AWS** — Amazon Web Services
- **BSS** — Blind Source Separation
- **CIFAR-10** — Canadian Institute for Advanced Research 10-class image dataset
- **CLI** — Command-Line Interface
- **CNN** — Convolutional Neural Network
- **CV** — Computer Vision
- **DFT** — Discrete Fourier Transform
- **FFT** — Fast Fourier Transform
- **Grad-CAM** — Gradient-weighted Class Activation Mapping
- **HTR** — Handwritten Text Recognition
- **I/O** — Input/Output
- **ICA** — Independent Component Analysis
- **LLM** — Large Language Model
- **LoRA** — Low-Rank Adaptation
- **MIME** — Multipurpose Internet Mail Extensions
- **ML** — Machine Learning
- **MNIST** — Modified National Institute of Standards and Technology handwritten-digit dataset
- **MSE** — Mean Squared Error
- **NLP** — Natural Language Processing
- **OCR** — Optical Character Recognition
- **OOP** — Object-Oriented Programming
- **PCA** — Principal Component Analysis
- **PEFT** — Parameter-Efficient Fine-Tuning
- **POS** — Part of Speech
- **PPNN / Double-P Double-N** — Paper-and-Pencil Neural Networks
- **ResNet-50** — 50-layer Residual Network
- **RLHF** — Reinforcement Learning from Human Feedback
- **RWKV** — Receptance Weighted Key Value
- **SVD** — Singular Value Decomposition
- **TDD** — Test-Driven Development
- **UI** — User Interface
- **w/o** — without
- **X2vec** — Catalog label for projects that learn vector representations of a chosen unit
- **T−V** — Kinetic energy minus potential energy, the common mechanical form of a Lagrangian
- **ZIP code** — United States postal code; ZIP originally meant Zone Improvement Plan
