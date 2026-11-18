# startup-course

모두의창업 바이브코딩 창업 과정에서 쓰는 스킬 묶음.

| 스킬 | 하는 일 |
|------|---------|
| market-diagnosis | 아이템을 시장·오퍼·가격·판매 네 축으로 진단하고, 가장 약한 고리와 검증할 가설, MVP로 풀 빈틈 후보를 뽑는다 |
| landing-page | 진단 리포트(또는 아이템 설명)로 가설 하나를 검증하는 사전 신청 랜딩페이지 기획서를 만든다. 코딩은 하지 않는다 |

흐름: market-diagnosis → landing-page → (Claude Code에서 랜딩 만들기·AXHub 배포) → (진단 리포트의 "MVP로 풀 빈틈"으로 MVP 초안)

## 설치 (Claude Code)

```
/plugin marketplace add jocoding-ax-partners/startup-course
/plugin install startup-course@startup-course
```

## 설치 (claude.ai 웹)

스킬 폴더를 하나씩 zip으로 묶어 올린다. zip 안에 폴더가 통째로 들어 있어야 한다.

```
cd skills
zip -r ../market-diagnosis.zip market-diagnosis -x "*.DS_Store"
zip -r ../landing-page.zip landing-page -x "*.DS_Store"
```

claude.ai → 설정 → 기능 → Skills → 스킬 업로드에서 두 파일을 하나씩 올린다.
