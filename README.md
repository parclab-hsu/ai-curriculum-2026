# 한성대학교 교육혁신센터 · AI융합교육과정 분석 (2026)

2026학년도 **AI융합교육과정 개편** 대상 트랙·학과(24개)를 대상으로 **기술 트렌드**와 **직무 역량 수요**를 분석하고, 트랙별 교육 목표·모듈형 전공교육과정을 제안한 MkDocs 사이트입니다. 채용·산업 동향은 LinkedIn·사람인·잡코리아·원티드 등 실제 채용 플랫폼과 산업 보고서 기반입니다.

- 🌐 사이트(배포 후): <https://parclab-hsu.github.io/ai-curriculum-2026/>
- 📊 원본 데이터/차트: [`parclab-hsu/tech-trends-2024-2026`](https://github.com/parclab-hsu/tech-trends-2024-2026)

## 구성

```
ai-curriculum-2026/
├── mkdocs.yml                 # MkDocs(Material) 설정 · 네비게이션
├── requirements.txt           # mkdocs-material
├── docs/
│   ├── index.md               # 홈 (전체 트랙 바로가기)
│   ├── overview.md            # 분석 개요 (거시 트렌드 + 개편 대상 지도)
│   ├── assets/charts/         # 추세선 차트 PNG
│   ├── design/                # 디자인대학 (AI디자인대학) 11개
│   ├── it/                    # IT공과대학 8개
│   └── ai/                    # 창의융합대학 (AI융합대학) 5개
└── .github/workflows/deploy.yml  # GitHub Pages 자동 배포
```

각 트랙/학과 페이지 구성: ① 개요 ② 산업·기술 트렌드 ③ 채용 동향 ④ 요구 직무 역량 ⑤ 대표 채용 기업 ⑥ 교육과정 개편 시사점 ⑦ 출처 ⑧ 교육 목표(예시) ⑨ 교육과정 구성·교수법 ⑩ 모듈형 전공교육과정.

## 로컬 미리보기

```bash
pip install -r requirements.txt
mkdocs serve          # http://127.0.0.1:8000
mkdocs build --strict # 정적 빌드(site/)
```

## 배포 (GitHub Pages)

1. GitHub에 `parclab-hsu/ai-curriculum-2026` 저장소 생성 후 push.
2. 저장소 **Settings → Pages → Build and deployment → Source: GitHub Actions** 선택.
3. `main` 브랜치 push 시 `.github/workflows/deploy.yml`가 자동 빌드·배포.

> 데이터 기준 2026-06. 수치 중 일부는 출처 보고값/추정값이 혼재하며, 본문에 '추정'으로 표기되어 있습니다.
