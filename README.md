# NLP_Project

<h2> Key Features</h2>

<ul>
  <li><strong> Fine-Tuned BERT-Based Models:</strong><br>
  Utilized pre-trained transformer models like <code>bert-base-uncased</code> and <code>distilbert-base-uncased</code> for the Question Answering task, fine-tuned on custom data.</li>

  <li><strong> Custom Dataset Preprocessing:</strong><br>
  Implemented detailed preprocessing logic to align context, question, and answer spans, including precise token-to-character offset mapping for accurate label alignment.</li>

  <li><strong> Transfer Learning:</strong><br>
  Leveraged the power of transfer learning by starting from pre-trained weights and adapting the models to a domain-specific question answering dataset.</li>

  <li><strong> Training and Evaluation:</strong><br>
  Trained the models using Hugging Face’s <code>Trainer</code> API and evaluated them with custom metrics such as F1 score and Exact Match (EM).</li>

  <li><strong> Loss Tracking:</strong><br>
  Monitored training and validation loss to diagnose underfitting, overfitting, and model generalization across epochs.</li>

  <li><strong> Testing on Unseen Data:</strong><br>
  Tokenized and evaluated the model on a held-out test set to simulate real-world usage and validate performance.</li>

  <li><strong> Model Checkpointing:</strong><br>
  Saved and reused trained models, enabling reloading for future evaluation or deployment without retraining.</li>

  <li><strong> Visualizations (Optional):</strong><br>
  Enabled visual analysis of model performance trends (e.g., training vs validation loss) to guide optimization.</li>

  <li><strong> Experimentation-Ready:</strong><br>
  Modular code structure allows easy experimentation with other transformer models (e.g., RoBERTa, ALBERT) and hyperparameter tuning.</li>
</ul>

<h2> Model Performance</h2>

<h3>BERT Model Results</h3>
<table>
  <thead>
    <tr>
      <th>Epoch</th>
      <th>Training Loss</th>
      <th>Validation Loss</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>1.232800</td>
      <td>2.420470</td>
    </tr>
    <tr>
      <td>2</td>
      <td>0.994700</td>
      <td>2.616735</td>
    </tr>
    <tr>
      <td>3</td>
      <td>0.511000</td>
      <td>3.290370</td>
    </tr>
  </tbody>
</table>

<h3>DistilBERT Model Results</h3>
<table>
  <thead>
    <tr>
      <th>Epoch</th>
      <th>Training Loss</th>
      <th>Validation Loss</th>
      <th>Start Accuracy</th>
      <th>End Accuracy</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>4.121600</td>
      <td>1.708325</td>
      <td>1.000000</td>
      <td>0.000000</td>
    </tr>
    <tr>
      <td>2</td>
      <td>3.666900</td>
      <td>1.799927</td>
      <td>0.510000</td>
      <td>0.000000</td>
    </tr>
    <tr>
      <td>3</td>
      <td>3.612600</td>
      <td>1.857204</td>
      <td>0.510000</td>
      <td>0.000000</td>
    </tr>
  </tbody>
</table>

