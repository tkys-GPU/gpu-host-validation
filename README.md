# gpu-host-validation

## Environment
- Ubuntu 22.04 LTS
- NVIDIA Driver 575.64.03 / CUDA 12.9
- RTX 4080 SUPER (PCIe Gen4 x16)

## Validation Results
- PyTorch / TensorFlow: successfully tested
- BandwidthTest: H2D = 24.1 GB/s, D2H = 26.3 GB/s (Gen4 x16, normal operation)
- dmesg: no uncorrected/fatal errors (only AER notifications enabled)
- 
### Framework Validation

- **PyTorch 2.3.0**
  - Version: 2.3.0
  - CUDA available: True
  - Status: ✅ Successfully tested, GPU recognized

- **TensorFlow 2.16.1**
  - Version: 2.16.1
  - Detected GPU: /physical_device:GPU:0
  - Status: ✅ Successfully tested, GPU recognized
  - Notes: Warnings about oneDNN, AVX/FMA optimizations, and NUMA node are environment-related and do not affect normal GPU usage

## Log Files
- [bandwidthTest_4080S_2025-08-24.log](logs/bandwidthTest_4080S_2025-08-24.log)
- [aer_check_4080S_2025-08-24.log](logs/aer_check_4080S_2025-08-24.log)
