# CNN Compression with SVD

This project demonstrates compressing CNN dense layers using Singular Value Decomposition (SVD) while maintaining high accuracy.

## Key Points

- **Network:** 4 convolutional layers + 2 dense layers; original test accuracy 99.19%.
- **Dense Layer Compression:** Weight matrix (1024×128) compressed with SVD for k = 16, 32, 64.
- **Results:** Up to 7× memory reduction with negligible accuracy loss.
- **Fine-Tuning:** Only the last layer retrained, restoring accuracy to or above original.
- **Biclustering:** No improvement; adds unnecessary computation.

## Recommended Setting

- **k = 32:** Good trade-off between compression (~72% memory savings) and accuracy (99.37% after fine-tuning).

## Applications

- Deploy CNNs on memory-constrained devices
- Reduce storage and energy requirements
