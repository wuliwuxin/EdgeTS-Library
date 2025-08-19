# Edge Intelligence for Time Series Library

**Edge Intelligence Time Series (EITS)** is an open‑source library for deep learning researchers and practitioners, **especially for resource‑constrained edge deployment on streaming time‑series** from IoT sensors, wearables, and industrial telemetry.

> **Tagline:** Train, compress, and deploy time‑series models that meet real‑world **latency/energy/memory** constraints—without sacrificing accuracy.

<!-- :triangular_fag_on_post:**News** (2024.10) We have included [[TimeXer]](https://arxiv.org/abs/2402.19072), which defined a practical forecasting paradigm: Forecasting with Exogenous Variables. Considering both practicability and computation efficiency, we believe the new forecasting paradigm defined in TimeXer can be the "right" task for future research. -->

## Why EITSLib?

* **Edge‑first**: Every component is designed with on‑device constraints in mind.
* **Task‑centric**: Unified APIs for **forecasting, anomaly detection, classification, and imputation**.
* **Production‑aware**: Built‑in profiling, compression, and portable export targets (ONNX/TFLite/WASM).


## Who is it for?

* Researchers prototyping new architectures for time series under edge constraints.
* Engineers building on‑device analytics for sensors, wearables, smart home/industry, robotics.
* Students needing a clean reference for end‑to‑end TS modeling from **data → training → compression → deployment**.

## What we provide

* **Unified Time‑Series Tasks**: `Forecasting`, `AnomalyDetection`, `Classification`, `Imputation` with consistent data/metric interfaces.
* **Edge‑Optimized Model Zoo**: Lightweight baselines and modern TS models with tiny variants (e.g., **TCN**, **LSTM/GRU**, **N‑BEATS/N‑HiTS**, **DLinear**, **TimesNet‑Tiny**, **PatchTST‑Lite**).
* **Streaming Data Pipelines**: Sliding/rolling windows, causal masks, online normalization, missing‑value handling, and chunked loaders for on‑device memory limits.
* **Compression Toolkit**: Quantization‑aware training (QAT), post‑training quantization (PTQ int8), structured pruning, knowledge distillation, early‑exit heads.
* **Resource‑Aware Training**: Multi‑objective and constraint‑aware training with knobs for **latency/params/energy** budgets.
* **Profiling & Evaluation**: FLOPs/params, CPU/ARM latency estimation, memory footprint, online metrics (delay‑aware MAE/MSE, F1 for anomalies, AUROC/PRC).
* **Deployment Paths**: Export to **ONNX**, **TFLite**, and **WebAssembly**; helper stubs for microcontroller integration.
* **Federated/Continual Options**: Simple **FedAvg** hooks, replay buffers, and drift detectors for non‑stationary streams.
* **Reproducible Recipes**: Reference configs and scripts for common datasets (ETT, UCR, M4, NAB, Electricity, Traffic).

> Dataset names are provided for convenience—loaders are implemented when licensing allows; otherwise helper scripts are included.

<!-- See our latest paper [[TimesNet]](https://arxiv.org/abs/2210.02186) for the comprehensive benchmark. We will release a real-time updated online version soon.

**Newly added baselines.** We will add them to the leaderboard after a comprehensive evaluation.
  - [x] **MultiPatchFormer** - A multiscale model for multivariate time series forecasting [[Scientific Reports 2025]](https://www.nature.com/articles/s41598-024-82417-4) [[Code]](https://github.com/thuml/Time-Series-Library/blob/main/models/MultiPatchFormer.py) -->
## Contact
In case of any questions, bugs, suggestions or improvements, please feel free to drop me at `xinwu5386@gmail.com` or open an issue.