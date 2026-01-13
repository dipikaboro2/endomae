# EndoMAE

EndoMAE is a masked autoencoder framework for representation learning in endoscopic images.

<p align="center">
  <img src="images/mae-endo.jpg" width="600">
</p>

### Will be updated after paper is published.

## Abstract
Large vision models (LVMs) pretrained on massive visual datasets have demonstrated strong transferability across downstream tasks such as classification, detection, and segmentation. This transferability makes them particularly effective in low-labeled data settings where representation learning from unlabeled data has emerged as a promising alternative to fully supervised approaches. In this work, we introduce EndoMAE, a self-supervised foundation model for endoscopic image analysis based on masked autoencoding. For pretraining, we curate a large-scale, high-quality dataset by automatically filtering and processing raw endoscopic video frames to retain only anatomically relevant regions and remove low-quality samples. This process yields 6.5 million endoscopic images, which are combined with publicly available data to form a corpus of over 10 million images for self-supervised pretraining. EndoMAE is trained to reconstruct masked image patches, encouraging the learning of rich, domain-specific representations without manual annotations or prompt engineering. We evaluate EndoMAE on endoscopic benchmarks that are fully disjoint from the pretraining datasets for image classification and polyp segmentation as downstream tasks. We compare EndoMAE with both supervised and self-supervised pretrained feature extractors. Compared to self-supervised baselines, EndoMAE achieves gains of up to 5.2\% F1 and 10.2\% dice score across the respective tasks, demonstrating strong cross-dataset generalization and task adaptability in low-annotation endoscopic imaging settings.

<!--
## 📄 Paper

**EndoMAE: A Foundation Model for Endoscopic Image Analysis via Self-Supervised Learning**

- Authors: D. Boro, Q. Chen, X. Liang, Y. Cao, B. Liu
- Conference / Journal: Accepted at SPIE Medical Imaging
- Year: 2026


If you find this work useful, please cite:

```bibtex
@article{endomae2026,
  title={EndoMAE: A Foundation Model for Endoscopic Image Analysis via Self-Supervised Learning},
  author={D. Boro, Q. Chen, X. Liang, Y. Cao, B. Liu},
  journal={SPIE, Medical Imaging},
  year={2026}
  --1!>
}

