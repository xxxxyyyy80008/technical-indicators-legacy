---
layout: default
title: Technical Indicators
nav_order: 1
has_children: true
has_toc: false
permalink: /indicators/
---


# Technical Indicators
{: .fs-7 }

**55+ production-ready implementations** with mathematical foundations and empirical validation.
{: .fs-5 .fw-300 }

[Source Code](https://github.com/xxxxyyyy80008/talib2025){: .btn .btn-primary .fs-3 .mb-2 .mb-md-0}{:target="_blank" rel="noopener noreferrer"}

---

## Quick Stats

| Metric | Value |
|:-------|:------|
| **Total Indicators** | 55 |
| **Categories** | 7 (Adaptive, Momentum, Trend, Volatility, Volume, Sentiment, DSP) |
| **Languages** | Python, NumPy/Pandas|
| **Documentation** | Full LaTeX formulas + parameter tuning guides |
| **Academic Sources** | 20+ TASC papers, Ehlers, Kaufman, DeMark |

---

## Highlights

 **Mathematical Modeling** — Fractal dimension, Hilbert transforms, Kalman filtering  
 **Signal Processing** — FIR filters, Hann windowing, Ehlers DSP techniques  
 **Statistical Methods** — Stochastic processes, volatility normalization, efficiency ratios  
 **Research Translation** — Academic papers → validated Python code  

---

##  Indicator Catalog

###  Adaptive Moving Averages (9)
*Self-adjusting algorithms based on volatility, volume, or fractal dimension*

| Indicator | Adaptation Method | Link |
|:----------|:------------------|:-----|
| FRAMA | Fractal dimension | [View](/technical-indicators-legacy/b_002_1_frama_intro/b_002_1_frama_intro.html) |
| VAMA | Volatility-based | [View](/technical-indicators-legacy/b_003_1_vama_intro/b_003_1_vama_intro.html) |
| MAMA | Hilbert Transform (MESA) | [View](/technical-indicators-legacy/b_037_1_mama_intro/b_037_1_mama_intro.html) |
| Kaufman ER | Efficiency ratio | [View](/technical-indicators-legacy/b_025_1_er_intro/b_025_1_er_intro.html) |
| RS_EMA | Relative strength | [View](/technical-indicators-legacy/b_038_1_rs-ema_intro_tasc202205_v2/b_038_1_rs-ema_intro_tasc202205_v2.html) |
| RS VolatAdj EMA | Volatility-adjusted RS | [View](/technical-indicators-legacy/b_039_1_rs-volat-adj-ema_intro_tasc202203/b_039_1_rs-volat-adj-ema_intro_tasc202203.html) |
| RS VA EMA | Volume-adjusted RS | [View](/technical-indicators-legacy/b_052_1_rs-va-ema_intro_tasc202210/b_052_1_rs-va-ema_intro_tasc202210.html) |
| TRAdj EMA | True range adjusted | [View](/technical-indicators-legacy/b_053_1_tr_adj_ema_tasc202301/b_053_1_tr_adj_ema_tasc202301.html) |
| RSIH | Hann windowing + RS | [View](/technical-indicators-legacy/b_043_1_rsih_intro_tasc202201/b_043_1_rsih_intro_tasc202201.html) |

**Key Formula (FRAMA):**

$$
\alpha = e^{-4.6(D-1)}, \quad D = \frac{\log(N_1+N_2)-\log(N_3)}{\log 2}
$$

---

###  Momentum Oscillators (13)
*Overbought/oversold detection and momentum strength measurement*

| Indicator | Range | Signal Threshold | Link |
|:----------|:-----:|:----------------|:-----|
| RSI | 0-100 | OB >70, OS <30 | [View](/technical-indicators-legacy/b_006_1_rsi_intro/b_006_1_rsi_intro.html) |
| Stochastic RSI | 0-1 | OB >0.8, OS <0.2 | [View](/technical-indicators-legacy/b_006_1_rsi_intro/b_006_1_rsi_intro.html) |
| IFT RSI | -1 to +1 | Sharpened signals | [View](/technical-indicators-legacy/b_006_1_rsi_intro/b_006_1_rsi_intro.html) |
| Connors RSI | 0-100 | Multi-component RSI | [View](/technical-indicators-legacy/b_012_1_crsi_intro/b_012_1_crsi_intro.html) |
| Breakout RSI (BRSI) | 0-100 | Breakout validation | [View](/technical-indicators-legacy/b_054_1_brsi_tasc201509/b_054_1_brsi_tasc201509.html) |
| Awesome Oscillator | ±∞ | Zero-line cross | [View](/technical-indicators-legacy/b_001_1_ao_intro/b_001_1_ao_intro.html) |
| CCI | ±∞ | OB >+100, OS <-100 | [View](/technical-indicators-legacy/b_007_1_cci_intro/b_007_1_cci_intro.html) |
| Williams %R | -100 to 0 | OB >-20, OS <-80 | [View](/technical-indicators-legacy/b_008_1_william-r_intro/b_008_1_william-r_intro.html) |
| Chande MO (CMO) | -100 to +100 | Zero-line momentum | [View](/technical-indicators-legacy/b_016_1_cmo_intro/b_016_1_cmo_intro.html) |
| Dynamic MI (DYMI) | 0-100 | Adaptive RSI | [View](/technical-indicators-legacy/b_018_1_dymi_intro/b_018_1_dymi_intro.html) |
| KDJ | 0-100+ | J-line extremes | [View](/technical-indicators-legacy/b_027_1_kdj_intro2/b_027_1_kdj_intro2.html) |
| Coppock Curve | ±∞ | Long-term bottoms | [View](/technical-indicators-legacy/b_013_1_copp_intro/b_013_1_copp_intro.html) |
| Greed & Fear (GFI) | 0-100 | Sentiment extremes | [View](/technical-indicators-legacy/b_055_1_gfi_tasc202210/b_055_1_gfi_tasc202210.html) |

---

### Trend Following (11)
*Directional movement and trend strength identification*

| Indicator | Type | Best For | Link |
|:----------|:-----|:---------|:-----|
| MACD | Oscillator | Trend + momentum | [View](/technical-indicators-legacy/b_005_1_macd_intro/b_005_1_macd_intro.html) |
| MACD-V | Oscillator | Volatility-normalized | [View](/technical-indicators-legacy/b_051_1_macd-v_intro_ssrn/b_051_1_macd-v_intro_ssrn.html) |
| VW MACD | Oscillator | Volume confirmation | [View](/technical-indicators-legacy/b_047_1_vw_macd_intro_tasc200910/b_047_1_vw_macd_intro_tasc200910.html) |
| Stochastic MACD | Oscillator | Bounded (0-100) | [View](/technical-indicators-legacy/b_040_1_stochastic-macd_intro_tasc201911/b_040_1_stochastic-macd_intro_tasc201911.html) |
| MADH | Oscillator | Hann-smoothed | [View](/technical-indicators-legacy/b_046_1_madh_intro_tasc202111/b_046_1_madh_intro_tasc202111.html) |
| ADX | 0-100 | Trend strength | [View](/technical-indicators-legacy/b_017_1_dmi_adx_intro/b_017_1_dmi_adx_intro.html) |
| DMH | Directional | Improved DMI | [View](/technical-indicators-legacy/b_042_1_dmh_intro_tasc202112/b_042_1_dmh_intro_tasc202112.html) |
| Vortex | Directional | VI+/VI- crossover | [View](/technical-indicators-legacy/b_019_1_vortex_intro_tasc201001/b_019_1_vortex_intro_tasc201001.html) |
| Aroon | 0-100 | Trend timing | [View](/technical-indicators-legacy/b_049_1_aroon_intro/b_049_1_aroon_intro.html) |
| Ichimoku Cloud | Multi-component | Complete system | [View](/technical-indicators-legacy/b_020_1_ichimoku-cloud_intro/b_020_1_ichimoku-cloud_intro.html) |
| Schaff Trend Cycle | 0-100 | Cycle oscillator | [View](/technical-indicators-legacy/b_024_1_schaff-trend-cycle_intro/b_024_1_schaff-trend-cycle_intro.html) |

---

###  Volatility & Bands (9)
*Price envelopes, breakout detection, and mean reversion*

| Indicator | Construction | Use Case | Link |
|:----------|:-------------|:---------|:-----|
| Bollinger Bands | SMA ± 2σ | Mean reversion | [View](/technical-indicators-legacy/b_004_1_bbands_intro/b_004_1_bbands_intro.html) |
| Keltner Channels | EMA ± 2×ATR | Breakouts | [View](/technical-indicators-legacy/b_015_1_keltner-channels_intro/b_015_1_keltner-channels_intro.html) |
| Donchian Channel | N-period high/low | Turtle strategy | [View](/technical-indicators-legacy/b_029_1_do_taq_intro/b_029_1_do_taq_intro.html) |
| Exp Deviation Bands | Exponential SD | Fast adaptation | [View](/technical-indicators-legacy/b_023_1_exponential-deviation-bands_intro_tasc201907/b_023_1_exponential-deviation-bands_intro_tasc201907.html) |
| Adaptive Price Zone | Dynamic zones | Volatility regimes | [View](/technical-indicators-legacy/b_048_1_apz_intro/b_048_1_apz_intro.html) |
| MA Bands (MAB/MABW) | Multi-MA + width | Band width signals | [View](/technical-indicators-legacy/b_044_1_mab_intro_tasc202108/b_044_1_mab_intro_tasc202108.html) |
| Choppiness Index | 0-100 | Trend vs. range | [View](/technical-indicators-legacy/b_014_1_chop_intro/b_014_1_chop_intro.html) |
| Wave PM | Energy model | Volatility energy | [View](/technical-indicators-legacy/b_022_1_wave-pm_intro/b_022_1_wave-pm_intro.html) |
| Value Chart | Detrended | Normalized price | [View](/technical-indicators-legacy/b_021_1_value-chart_intro/b_021_1_value-chart_intro.html) |

**Squeeze Detection:** BB inside KC → Contraction phase

---

###  Volume-Based (5)
*Confirmation via volume analysis and money flow*

| Indicator | Metric | Interpretation | Link |
|:----------|:-------|:---------------|:-----|
| Money Flow Index | Volume-weighted RSI | Buying/selling pressure | [View](/technical-indicators-legacy/b_009_1_mfi_intro/b_009_1_mfi_intro.html) |
| Chaikin Money Flow | AD accumulation | Money flow strength | [View](/technical-indicators-legacy/b_010_1_chaikin-mf_intro/b_010_1_chaikin-mf_intro.html) |
| Chaikin Oscillator | MACD of AD Line | Momentum of accumulation | [View](/technical-indicators-legacy/b_011_1_chaikin-oscillator_intro/b_011_1_chaikin-oscillator_intro.html) |
| Volume Pos/Neg (VPN) | High-volume breakouts | Breakout confirmation | [View](/technical-indicators-legacy/b_045_1_vpn_intro_tasc202104/b_045_1_vpn_intro_tasc202104.html) |

---

###  Sentiment & Breadth (6)
*Market psychology and relative strength analysis*

| Indicator | Measures | Signal | Link |
|:----------|:---------|:-------|:-----|
| Psychological Line | % bullish days | Contrarian | [View](/technical-indicators-legacy/b_032_1_psy_intro/b_032_1_psy_intro.html) |
| Elder-Ray (Bull/Bear) | Buying/selling power | $$\text{Bull} = H - EMA_{13}$$ | [View](/technical-indicators-legacy/b_033_1_ebbp_intro/b_033_1_ebbp_intro.html) |
| BRAR | Sentiment willingness | Chinese indicator | [View](/technical-indicators-legacy/b_035_1_brar_intro/b_035_1_brar_intro.html) |
| RSMK | Mansfield RS | Stock vs. benchmark | [View](/technical-indicators-legacy/b_026_1_rsmk_intro_tasc202003/b_026_1_rsmk_intro_tasc202003.html) |
| Tom DeMark TD9 | Exhaustion count | 9/13 sequences | [View](/technical-indicators-legacy/b_030_1_demark_intro_tasc201109/b_030_1_demark_intro_tasc201109.html) |
| ASI | Swing index | Accumulation | [View](/technical-indicators-legacy/b_031_1_asi_intro/b_031_1_asi_intro.html) |

---

###  Signal Processing (4)
*Digital signal processing techniques from electrical engineering*

| Indicator | Technique | Author/Source | Link |
|:----------|:----------|:--------------|:-----|
| Ehlers Decycler | High-pass filter | John Ehlers | [View](/technical-indicators-legacy/b_034_1_decycler-oscillator_intro_tasc201509/b_034_1_decycler-oscillator_intro_tasc201509.html) |
| Hann FIR Filter | Windowed FIR | DSP/TASC | [View](/technical-indicators-legacy/b_041_1_fir-windowing_intro_tasc202109/b_041_1_fir-windowing_intro_tasc202109.html) |
| BBI | Multi-MA composite | — | [View](/technical-indicators-legacy/b_036_1_bbi_intro/b_036_1_bbi_intro.html) |
| XSII | — | — | [View](/technical-indicators-legacy/b_028_1_xs2_intro/b_028_1_xs2_intro.html) |

---
