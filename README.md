# FEMA P695 (ATC-63) Far-Field Ground Motion Dataset

A curated academic repository for the FEMA P695 (ATC-63) far-field ground-motion dataset, including 22 pairs of horizontal acceleration records, normalized acceleration time-history curves, and 5%-damped elastic response spectra.

## Overview

This repository provides an organized and analysis-ready version of the FEMA P695 (ATC-63) far-field ground-motion set for earthquake engineering research. The dataset includes 22 pairs of horizontal ground-motion records, corresponding to 44 horizontal acceleration components. These records are commonly used in nonlinear response-history analysis, incremental dynamic analysis, collapse assessment, and seismic performance evaluation of building structures.

This repository is intended to improve accessibility and reproducibility for academic research. The provided data include processed acceleration time histories, normalized acceleration time histories, and 5%-damped elastic response spectra.

## Ground Motion Set

The FEMA P695 (ATC-63) far-field ground-motion set consists of 22 pairs of horizontal records. Each pair contains two orthogonal horizontal components from the same earthquake station. Therefore, the complete far-field set includes:

```text
22 ground-motion pairs × 2 horizontal components = 44 acceleration time histories
```

## Normalized Acceleration Records

The normalized acceleration time histories are obtained by dividing each acceleration record by its maximum absolute value:

```text
a_norm(t) = a(t) / max(|a(t)|)
```

After normalization, the maximum absolute value of each record is equal to 1.0:

```text
max(|a_norm(t)|) = 1.0
```

These normalized records are useful when users need to apply their own intensity scaling factors, such as PGA, spectral acceleration, or IDA-based scale factors.

## 5%-Damped Elastic Response Spectra

This repository also provides 5%-damped elastic response spectra for the ground-motion records. These spectra are commonly used in earthquake engineering for ground-motion characterization, record scaling, and comparison with design spectra.

Unless otherwise stated, the response spectra are calculated for a damping ratio of:

```text
ξ = 5%
```

Users should verify the period range, period interval, damping ratio, and numerical algorithm before using the spectra in formal publications or engineering applications.

## Important Notes

1. The original acceleration records may have different time steps, numbers of points, durations, and component directions.
2. The normalized records do not preserve the original PGA values.
3. The response spectra should be recalculated if users modify the records, apply filtering, baseline correction, or additional scaling.
4. Users should always verify the metadata before using the records in nonlinear dynamic analysis.
5. This repository is intended for academic and reproducible research purposes.

## Disclaimer

This repository is not an official distribution of FEMA, ATC, PEER, or the University of California, Berkeley. It is not affiliated with, endorsed by, or maintained by these organizations.

The ground-motion records and derived data are provided for academic and reproducible research purposes. Users are responsible for verifying the accuracy, completeness, units, scaling factors, metadata, and applicability of the records before using them in structural analysis, engineering design, or academic publication.

The license of this repository applies only to the scripts and documentation created for this repository. It does not imply ownership of, or licensing rights over, the original PEER/NGA ground-motion records. Users should ensure that their use and redistribution of the original and processed ground-motion data comply with the terms and conditions of the original data providers.

## License

The scripts and documentation in this repository may be released under the MIT License, unless otherwise stated.

The original and derived ground-motion data are subject to the terms and conditions of their original data providers. The repository license does not override those terms.

---

# FEMA P695 (ATC-63) 远场地震动数据集

本仓库是一个精选的学术数据仓库，用于整理和存储 FEMA P695 (ATC-63) 远场地震动数据集，包括 22 对水平加速度记录、归一化加速度时程曲线以及 5% 阻尼比弹性反应谱。

## 简介

本仓库提供经过整理、便于分析使用的 FEMA P695 (ATC-63) 远场地震动数据集，主要服务于地震工程领域的学术研究。该数据集包括 22 对水平地震动记录，即 44 条水平加速度分量。这些地震动记录常用于非线性动力时程分析、增量动力分析、结构倒塌评估以及建筑结构抗震性能评价。

本仓库的主要目的是提高数据使用的便利性和研究结果的可重复性。仓库中包括处理后的加速度时程、归一化加速度时程以及 5% 阻尼比弹性反应谱。

## 地震动记录集

FEMA P695 (ATC-63) 远场地震动集由 22 对水平地震动记录组成。每一对地震动包括同一台站的两个正交水平分量。因此，完整远场地震动集包括：

```text
22 对地震动 × 2 个水平分量 = 44 条加速度时程
```

## 归一化加速度记录

归一化加速度时程通过将每条加速度记录除以其最大绝对值获得：

```text
a_norm(t) = a(t) / max(|a(t)|)
```

归一化后，每条记录的最大绝对值均为 1.0：

```text
max(|a_norm(t)|) = 1.0
```

归一化地震动适用于用户希望自行施加强度缩放系数的情况，例如按照 PGA、谱加速度或 IDA 分析中的比例系数进行缩放。

## 5% 阻尼比弹性反应谱

本仓库还提供地震动记录对应的 5% 阻尼比弹性反应谱。该反应谱常用于地震动特性分析、地震动调幅以及与设计反应谱进行对比。

除非特别说明，反应谱计算采用的阻尼比为：

```text
ξ = 5%
```

用户在正式发表论文或工程应用前，应核查反应谱的周期范围、周期间隔、阻尼比和数值计算方法。

## 重要说明

1. 原始加速度记录可能具有不同的时间步长、数据点数、持续时间和分量方向。
2. 归一化记录不再保留原始 PGA 数值。
3. 如果用户对地震动进行了滤波、基线校正或额外缩放，应重新计算反应谱。
4. 用户在进行非线性动力分析前，应核查每条记录的元数据。
5. 本仓库主要用于学术研究和可重复性研究。

## 免责声明

本仓库不是 FEMA、ATC、PEER 或加州大学伯克利分校的官方数据发布渠道，也不隶属于、代表或受到上述机构认可。

本仓库中的地震动记录及其派生数据仅用于学术研究和可重复性研究。用户在将其用于结构分析、工程设计或学术发表前，应自行核查数据的准确性、完整性、单位、缩放系数、元数据和适用性。

本仓库的许可证仅适用于本仓库作者创建的脚本和文档，并不表示本仓库拥有原始 PEER/NGA 地震动记录的所有权或授权许可。用户应确保其对原始及处理后地震动数据的使用和再分发符合原始数据提供方的相关条款。

## 许可证

除非另有说明，本仓库中的脚本和文档可采用 MIT License 发布。

原始地震动数据及其派生数据受原始数据提供方的相关条款约束。本仓库许可证不能覆盖或替代原始数据提供方的条款。
