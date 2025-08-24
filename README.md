# gpu-host-validation

## Environment
- Ubuntu 22.04 LTS
- NVIDIA Driver 575.64.03 / CUDA 12.9
- RTX 4080 SUPER (PCIe Gen4 x16)

## Validation Results
- PyTorch / TensorFlow: successfully tested
- BandwidthTest: H2D = 24.1 GB/s, D2H = 26.3 GB/s (Gen4 x16, normal operation)
- dmesg: no uncorrected/fatal errors (only AER notifications enabled)

## Log Files
- [bandwidthTest_4080S_2025-08-24.log](logs/bandwidthTest_4080S_2025-08-24.log)
- [aer_check_4080S_2025-08-24.log](logs/aer_check_4080S_2025-08-24.log)
