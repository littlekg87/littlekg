<a id="korean"></a>

**한국어** · [English](#english)

# 세종실록지리지 자료·코드 (2025년 논문 판)

> **이 브랜치는 더 이상 갱신되지 않습니다.**
> 최신 자료는 **[littlekg87/Sejong_Sillok_Jiriji](https://github.com/littlekg87/Sejong_Sillok_Jiriji)** 에 있습니다.

## 이 브랜치는 무엇인가

아래 논문을 작성할 때 사용한 자료와 코드이다.

> 김근하·우동현, 「조선 전기 군역의 형평성 측정: GIS와 불평등 지표를 활용한 디지털 인문학적 분석」, 『역사와 현실』 137, 2025, 247~290쪽.
> DOI: [10.35865/ywh.2025.06.136.247](https://doi.org/10.35865/ywh.2025.06.136.247)

**논문에 실린 수치를 그대로 재현하려면 이 브랜치의 자료를 써야 한다.** 그래서 옛 판이지만 지우지 않고 그대로 둔다.

```
Data/       원자료(2nd_wda_400.xml)와 호·구·군정 추출·변환 결과
Outcomes/   논문에 실린 산점도·피어슨 상관 행렬·지도의 출력본
code/       한자 수치 추출과 아라비아 숫자 변환 코드
```

## 새 저장소로 옮긴 까닭

논문 이후 지리지의 군정 기록을 원문 및 원전 이미지와 전수 대조하면서 여섯 건을 교정하였다. 그 결과 일부 수치가 달라졌다.

| | 이 브랜치 (2025년 논문 판) | 새 저장소 (현재 판) |
|---|---|---|
| 분석 단위 | 335행 | 334개 군현 |
| 군정 합계 | 102,539명 | 102,671명 |
| 구 합계 | 735,223명 | 735,950명 |
| 군정 대 호 비율의 지니계수 | 0.293 | 0.282 |

주요 교정은 남원도호부·구례현·회양도호부의 군정 누락 보완, 부령도호부의 군정 확정, 나주목의 구 교정, 경원도호부 중복 기사 처리이다. 어느 군현을 무엇에서 무엇으로 왜 고쳤는지는 새 저장소의 [`data/provenance.md`](https://github.com/littlekg87/Sejong_Sillok_Jiriji/blob/main/data/provenance.md) 3절에 적어 두었다.

새 저장소는 자료를 한자리에 모으고 컬럼 정의와 교정 내역을 문서로 갖추었으며, 병종별 인원과 공간 정보까지 담는다. 앞으로의 갱신은 그곳에서 이루어진다.

## 어느 쪽을 써야 하는가

| 목적 | 쓸 것 |
|---|---|
| 2025년 논문의 수치를 재현하려는 경우 | **이 브랜치** |
| 지리지 자료로 새 분석을 하려는 경우 | **[새 저장소](https://github.com/littlekg87/Sejong_Sillok_Jiriji)** |

## 인용

새 저장소의 자료를 인용하실 때에는 그곳의 「인용」 항목을 따라 주십시오. 이 브랜치의 자료를 쓰신 경우에는 위 논문을 인용하고, 자료의 출처를 이 브랜치로 밝혀 주십시오.

---

<a id="english"></a>

[한국어](#korean) · **English**

# Sejong Sillok Jiriji Data and Code (2025 article version)

> **This branch is no longer updated.**
> The current dataset lives at **[littlekg87/Sejong_Sillok_Jiriji](https://github.com/littlekg87/Sejong_Sillok_Jiriji)**.

## What this branch is

The data and code used for the following article.

> Kunha KIM and Donghyun WOO, "Measuring Equity in Early Joseon Military Service: A Digital Humanities Analysis Using Geographic Information Systems (GIS) and Inequality Indicators," *Yōksa wa Hyŏnsil* 137 (2025): 247–290.
> DOI: [10.35865/ywh.2025.06.136.247](https://doi.org/10.35865/ywh.2025.06.136.247)

**To reproduce the figures published in that article, use the data in this branch.** It is kept as it was for that reason.

```
Data/       source XML and the extracted/converted household, population, and conscript tables
Outcomes/   the scatter plot, Pearson correlation matrix, and map as published
code/       extraction of Sino-Korean numerals and conversion to Arabic numerals
```

## Why the work moved

After the article appeared, the military registration entries were collated in full against the original text and facsimile images, and six corrections were made. Some figures changed as a result.

| | This branch (2025 article) | New repository (current) |
|---|---|---|
| Units of analysis | 335 rows | 334 counties |
| Total conscripts | 102,539 | 102,671 |
| Total population (*gu*) | 735,223 | 735,950 |
| Gini of conscripts per household | 0.293 | 0.282 |

The corrections concern omitted conscript figures for Namwon, Gurye, and Hoeyang; the conscript total for Buryeong; the population figure for Naju; and the duplicate entry for Gyeongwon. Section 3 of [`data/provenance.md`](https://github.com/littlekg87/Sejong_Sillok_Jiriji/blob/main/data/provenance.md) in the new repository records each of them.

The new repository gathers the data in one place with a codebook and a provenance record, and extends it to troop-type figures and spatial measures. All further work happens there.

## Which to use

| Purpose | Use |
|---|---|
| Reproducing the figures in the 2025 article | **this branch** |
| New analysis of the *Jiriji* data | **[the new repository](https://github.com/littlekg87/Sejong_Sillok_Jiriji)** |
