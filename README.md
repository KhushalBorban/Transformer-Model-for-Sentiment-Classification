**Transformer Models for Sentiment Classification**

This project explores different Transformer-based approaches for financial sentiment analysis using the Finance PhraseBank Dataset. The models classify financial sentences into sentiment categories, with performance compared across a custom Transformer, PyTorch’s TransformerEncoderLayer, and BERT transfer learning.

**Features**

Custom Transformer Model: Implemented from scratch, achieving 73.28% accuracy.
PyTorch TransformerEncoderLayer: Improved performance with 77.89% accuracy and stronger generalization.
BERT Transfer Learning: Applied pre-trained BERT with a frozen encoder, achieving 81.88% accuracy with balanced precision-recall.
Comparative Analysis: Benchmarked different transformer variants for trade-offs in accuracy, precision, and generalization.

**Dataset**

Finance PhraseBank
Contains short financial news statements annotated with sentiment labels (Positive / Negative / Neutral).
Widely used for benchmarking sentiment classification in finance.

**Implementation**

Models
Custom Transformer
Implemented scaled dot-product attention, positional encoding, and multi-head attention from scratch.
Trained end-to-end on Finance PhraseBank.
PyTorch TransformerEncoderLayer
Leveraged PyTorch’s built-in encoder layer for improved stability and training efficiency.
Boosted precision and generalization compared to custom model.
BERT Transfer Learning
Pre-trained BERT-base with encoder layers frozen.
Fine-tuned classification head for sentiment detection.
Achieved highest accuracy (81.88%) with balanced precision-recall.

**Results**

Model	Accuracy	Precision-Recall Balance	Notes
Custom Transformer	73.28%	Moderate	From-scratch implementation
PyTorch TransformerEncoder	77.89%	Improved precision	Better generalization
BERT (Frozen Encoder)	81.88%	Balanced	Best trade-off between accuracy & recall
