---
hide_table_of_contents: false
pagination_prev: null
pagination_next: null
---

# 研究プログラム

## 確率微分方程式における同定と生成の理論

A theory of identification and generation in stochastic differential equations

---

## 概要

軌道やスナップショットとして観測されたデータから，確率過程を動かしている生成器（ドリフト・ポテンシャル）を遡って**同定**する（逆問題）．そして，同定した確率微分方程式（SDE）から望みの分布を**生成**する（順問題）．本プログラムは，この二つの理論を共通の数学的土台の上で発展させることを目指しています．

Identify, from observed trajectories and snapshots, the generator driving a stochastic process (the inverse problem), and generate target distributions from the identified SDE (the forward problem) — this program develops the two theories on a common mathematical foundation.

---

## 背景

確率過程の**逆問題**（生成器の同定：逆確率制御・ドリフト推定）と**順問題**（生成モデルの誤差解析）は，これまで別々の研究共同体で発展してきました．しかし両者の数学的な核は同一であり，**Schrödinger橋・h-path過程・Doob変換・前進後退確率微分方程式（FBSDE）** という共通言語の上で動いています．

当研究室は，この共通言語の上で逆側（逆確率制御）と順側（拡散生成モデルの収束解析）の双方の結果を得てきました．本プログラムは，両者を「同定された同一のSDE」を軸に発展させるものです．

---

## 三つの課題

1. **輸送** — 逆確率制御と（確率）最適輸送・Schrödinger問題の関係を，古典的な場合を特殊例として含む一般的な枠組みとして確立する．
2. **生成** — 同定したSDEを前進過程とするサンプリング（拡散モデル型生成）の誤差解析を確立し，DDPM型の収束理論を一般のドリフトへ拡張する．
3. **連結** — 同定の出力が生成の誤差保証を定量的に支配する「**同定→生成の誤差伝播関係**」を確立する．これが本プログラムの核心となる課題である．

方法論の中核は，分布への制約を**再生核ヒルベルト空間（RKHS）の距離**として定式化し，**不偏推定量**で標本から解くことにあります．深層学習的手法が欠く**有限標本保証と収束レート**（適切性・劣最適ギャップ・概収束）を備える点が，本プログラムの独自性です．理論の実証として，Langevin方程式の同定を公開の生態データ（動物行動軌道）で行い，同定から生成までを一気通貫で検証します．

---

## 代表的な成果

**同定（逆問題）側**

- 逆確率最適制御の適切性と数値解法 — [Automatica 149 (2023), 110831](https://doi.org/10.1016/j.automatica.2022.110831)
- 一般化シュレディンガー問題による逆確率制御 — [Systems & Control Letters 218 (2026), 106614](https://doi.org/10.1016/j.sysconle.2026.106614)
- Δt-バイアスフリーなドリフトポテンシャル同定 — [arXiv:2610.04268](https://arxiv.org/abs/2610.04268) [[code](https://github.com/yumiharu-nakano/inverse-drift-potential)]

**輸送側**

- カーネル法によるシュレディンガー橋 — Jpn. J. Ind. Appl. Math. 43 (2026), 46 [[arXiv:2310.14522](https://arxiv.org/abs/2310.14522)] [[code](https://github.com/yumiharu-nakano/kernelSB)]
- ヒルベルト空間埋め込みによる多周辺最適輸送 — Statist. Comput. 36 (2026), 118 [[arXiv:2412.03478](https://arxiv.org/abs/2412.03478)] [[code](https://github.com/yumiharu-nakano/kernelMMOT)]
- 連続周辺最適輸送のメッシュフリー・カーネル法 — [arXiv:2604.24226](https://arxiv.org/abs/2604.24226) [[code](https://github.com/yumiharu-nakano/alltimeOT)]

**生成（順問題）側**

- 離散時間DDPMの構造・収束解析 — [arXiv:2406.01320](https://arxiv.org/abs/2406.01320)
- カーネル型ポテンシャル平均場ゲームと不偏ランダムフーリエU統計量 — [arXiv:2605.29371](https://arxiv.org/abs/2605.29371) [[code](https://github.com/yumiharu-nakano/kernelMFG-RFU)]

**土台（数値解析）**

- 完全非線形放物型方程式のメッシュフリー選点法の収束 — Numer. Math. 136 (2017), 703–723
- 非有界領域上のHJB方程式に対するカーネル法・NN法の収束 — [arXiv:2610.09299](https://arxiv.org/abs/2610.09299) [[code](https://github.com/yumiharu-nakano/hjb-residual-methods)]

論文の完全なリストは[トップページ](/)をご覧ください．

---

## 研究系統樹

研究全体の流れと，各分野が統合プログラムへ合流していく様子を系統樹として可視化しています．

▶︎ [**研究系統樹を見る**](https://yumiharu-nakano.github.io/nakano-lab/tree.html)
