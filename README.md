# scaleiq_google_patents
a model trained by Google on 100M+ patents. Based on anferico/bert-for-patents

Huggingface link: https://api-inference.huggingface.co/models/anferico/bert-for-patents

To upload the model into the ScaleiQ_AI_Engine copy and paste de following under 
the dashboard dev tool:


POST /_plugins/_ml/models/_upload
{
  "name": "anferico/bert-for-patents",
  "version": "1.0.0",
  "description": "ScaleiQ Google Patents model",
  "model_format": "TORCH_SCRIPT",
  "model_config": {
    "model_type": "bert",
    "embedding_dimension": 1024,
    "framework_type": "sentence_transformers"
  },
   "url": "https://github.com/scaleiQLLModels/scaleiq_google_patents.git
