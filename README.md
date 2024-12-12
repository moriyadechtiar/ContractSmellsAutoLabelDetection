

  <h1>Contract Smells Auto Label & Detection</h1>

  <!-- Project Description -->
  <section id="project-description">
    <h2>Project Description</h2>
    <p>
      The <strong>Contract Smells Auto Label & Detection</strong> project employs advanced Natural Language Processing (NLP) techniques and machine learning models to identify and classify "contract smells" within legal documents. Inspired by the concept of "code smells" in software engineering, contract smells represent problematic patterns in legal contracts that may lead to misunderstandings, inefficiencies, or legal ambiguities.
    </p>
    <p>
      This project explores automated labeling methods and possible enhancements with minimal human labels, and examine transformer models with different levels of domain and task knowledge. The project aims to develop insights on datasets creation with automated labeling, as well as explore detection success on different types of Contract Smells and with the selected models.
    </p>
  </section>

  <!-- Repository Structure -->
  <section id="repository-structure">
    <h2>Repository Structure</h2>
    <pre><code>Contract-Smells-Detection/
├── auto_label.py
├── dataset_explore.py
├── pca_explore.py
├── cuadlegalbert_singleclass_detection_classimbalance_hpft.py
├── cuadlegalbert_multiclass_detection_classimbalance_hpft.py
├── cuadlegalbert_contract_smells_detection_hl_autol.py
├── hf_prompt_adjust.py
├── README.html
└── requirements.txt
    </code></pre>
  </section>

  <!-- Each File Highlights -->
  <section id="file-highlights">
    <h2>File Highlights</h2>
    <ul>
      <li>
        <strong>auto_label.py</strong>: Automates the labeling of contract clauses by identifying predefined contract smells using 3 different sets of prompt definitions.
      </li>
      <li>
        <strong>dataset_explore.py</strong>: Conducts exploratory data analysis (EDA) on labeled datasets to understand distributions, correlations, and class imbalances.
      </li>
      <li>
        <strong>pca_explore.py</strong>: Performs Principal Component Analysis (PCA) on clause embeddings to visualize data in a reduced dimensional space.
      </li>
      <li>
        <strong>cuadlegalbert_singleclass_detection_classimbalance_hpft.py</strong>: Fine-tunes CuadLegalBERT for single-class contract smells detection, addressing class imbalance and optimizing hyperparameters.
      </li>
      <li>
        <strong>cuadlegalbert_multiclass_detection_classimbalance_hpft.py</strong>: Extends the single-class approach to handle multiple contract smells simultaneously, optimizing hyperparameters.
      </li>
      <li>
        <strong>cuadlegalbert_contract_smells_detection_hl_autol.py</strong>: Integrates human-labeled and auto-labeled datasets to enhance model robustness and evaluation accuracy.
      </li>
      <li>
        <strong>hf_prompt_adjust.py</strong>: Enhances auto labeling prompts using few-shot examples selected from our most inaccurate predictions made, to improve classification accuracy for specific contract smells.
      </li>
    </ul>
  </section>

  <!-- Configuration -->
  <section id="configuration">
    <h2>Configuration</h2>
    <p>To execute the project effectively, the following API keys and environment variables are required:</p>
    <ul>
      <li>
        <strong>OpenAI API Key</strong>: Access GPT models for automated labeling and few-shot classification.
      </li>
      <li>
        <strong>Hugging Face API Key</strong>: Required for accessing Hugging Face models and datasets.
      </li>
      <li>
        <strong>Weights & Biases (WANDB) API Key</strong>: Enables experiment tracking and logging for hyperparameter fine-tuning.
      </li>
    </ul>
  </section>

