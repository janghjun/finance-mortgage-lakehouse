---

## `de-finance-mortgage-lakehouse`

# 💰 Finance Data Lakehouse (Mortgage/Loan)

## 프로젝트 개요
모기지/대출 성과 데이터를 기반으로 Delta/Iceberg 파이프라인을 구축한 프로젝트입니다.  
dbt Metrics를 통해 금융 KPI를 정의하고, Tableau/Power BI와 연동합니다.

---

## 아키텍처
- Source: Fannie Mae Loan Performance
- Ingestion: Apache Airflow + AWS Glue
- Storage: AWS S3 + Delta Lake / Iceberg
- Transformation: dbt (증분 모델 + 스냅샷)
- Data Quality: Great Expectations
- Semantic Layer: dbt Metrics
- Visualization: Tableau / Power BI

---

## 주요 기능
- 대출 데이터 적재 및 정제
- KPI: 연체율, 상환율, CPR/CRR 지표
- BI 대시보드 연계

---

## 결과물
- Tableau 대시보드 (연체율 시각화)
- GX 데이터 품질 리포트
- dbt 문서 사이트

---

## 향후 개선
- CDC 기반 실시간 파이프라인 (Debezium)
- ElasticSearch 기반 금융 데이터 검색 서비스
