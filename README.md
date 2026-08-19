# wafer-defect-visualization
웨이퍼 불량 패턴 시각화 및 FDC 리포팅 툴
# Wafer Defect Visualization & FDC Toolkit

웨이퍼 불량 패턴을 시각화하고 FDC(Fault Detection & Classification) 관점에서 해석하는 데이터 시각화 프로젝트입니다.

## 🔗 Live Demo

- [산점도 행렬 (Scatter Matrix)](https://hyunsle.github.io/wafer-defect-visualization/scatter_matrix.html)
- [웨이퍼 히트맵 (Wafer Heatmap)](https://hyunsle.github.io/wafer-defect-visualization/wafer_heatmap.html)

## 📌 프로젝트 개요

반도체 양산 공정에서는 웨이퍼 상의 불량 위치 패턴(Ring, Center, Scratch, Random 등)이 특정 공정 이슈와 연결되는 경우가 많습니다. 이 프로젝트는 합성 웨이퍼 데이터를 기반으로:

- 불량 패턴별 웨이퍼 맵 시각화
- 반경 평균·각도 집중도 기반 불량 패턴 자동 분류
- 배치 단위 PDF 리포트 자동 생성
- Plotly 기반 인터랙티브 산점도 행렬·히트맵

을 구현하여, 단순 시각화를 넘어 "패턴 → 원인 해석"으로 이어지는 FDC 워크플로우를 구성했습니다. 예를 들어 Ring 형태 불량은 증착 균일도 문제와, Scratch 형태는 이송/핸들링 이슈와 연결지어 해석하는 방식입니다.

## 🛠 Tech Stack

- Python (pandas, numpy)
- Matplotlib (정적 웨이퍼 맵)
- Plotly (인터랙티브 산점도 행렬, 히트맵)
- ReportLab (PDF 배치 리포트)

## 🔗 Related Project

실제 UCI SECOM 반도체 제조 데이터를 활용한 수율 예측 ML 프로젝트는 별도 레포에서 확인하실 수 있습니다.
👉 [secom-yield-prediction](https://github.com/hyunsle/secom-yield-prediction)

두 프로젝트는 각각 **모델링(수율 예측)**과 **시각화/모니터링(불량 패턴 해석)**이라는 반도체 데이터 분석의 서로 다른 축을 다룹니다.
