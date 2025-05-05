# Problem Definition
Current image retrieval systems predominantly rely on large, pretrained models such as CLIP or BERT, which can introduce limitations around interpretability, modularity, and data privacy—especially for organizations needing internal or domain-specific solutions. Furthermore, most systems treat search as a single-directional task (e.g., text-to-image only), limiting flexibility. This project aims to develop a lightweight, modular neural model for multimodal retrieval from scratch, without relying on pretrained encoders. The system is designed to handle three core tasks: (1) retrieving relevant images from text queries, (2) enabling image-to-image retrieval through caption generation, and (3) learning a shared embedding space for unified cross-modal retrieval. This approach provides a deeper understanding of the mechanics of sentence-image alignment while offering the potential for multilingual and customizable extensions in the future.

Through this project we have tried to attempt all three. The following notebook has the 3 trials in the following sequence-

Retrieve images based on comparing captions with the query
Captioning images received which can be tied back to the first approach and retrieve images
Image retrieval from a joint embedding space of both captions and images in the data set.
