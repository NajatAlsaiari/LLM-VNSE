# LLM-VNSE: Calibrated and Adaptive Listwise Ranking with LLMs for QoS-Aware Volunteer Node Selection

Reproducibility artefacts for the paper:
> "Calibrated and Adaptive Listwise Ranking with Large Language Models for Quality-of-Service-Aware Volunteer Node Selection in Fog Computing"

## Repository Contents

| Notebook | Description |
|----------|-------------|
| `dataset_preparation_all_schemes.ipynb` | Generates four QoS weight scheme datasets (A, B, C, D) from QWS Dataset 2.0 |
| `VBFC_synthetic_dataset_generator.ipynb` | Constructs the volunteer-fog synthetic dataset using CloudSimPlus 6.3.0 and Markov-modelled availability |
| `calibrated_listwise.ipynb` | Implements calibrated listwise ranking with confidence-gated selection and TOPSIS fallback |
| `dynamic_adaptation_experiment.ipynb` | Evaluates four orchestrators across a two-phase SLA shift trace (Scheme B → Scheme C) |

## Fine-tuned Model Adapters

All 12 QLoRA fine-tuned adapters (3 models × 4 schemes) are available on HuggingFace:
- [Llama 3.1 8B](https://huggingface.co/NajatAlsa/llama-scheme-a)
- [Qwen 2.5 7B](https://huggingface.co/NajatAlsa/qwen-scheme-a)
- [Mistral 7B](https://huggingface.co/NajatAlsa/mistral-scheme-a)

## Citation

```bibtex
@article{alsaiari-llmvnse,
  title={Calibrated and Adaptive Listwise Ranking with Large Language Models for Quality-of-Service-Aware Volunteer Node Selection in Fog Computing},
  author={Alsaiari, Najat and Hussain, Farookh},
  year={2026}
}
```
