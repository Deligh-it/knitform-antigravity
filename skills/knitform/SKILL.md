---
name: knitform
description: KNITFORM(대바늘·코바늘 뜨개 도안 및 패턴 스튜디오)의 원격 MCP 엔드포인트 연동 가이드.
---

# KNITFORM Antigravity Skill

KNITFORM은 대바늘·코바늘 도안을 웹 브라우저에서 설계하고 편집할 수 있는 뜨개 도안 제작 도구(Pattern Studio)입니다.
이 스킬은 Antigravity 에이전트가 원격 MCP 엔드포인트(`https://knitform.deligh-it.app/mcp`)와 통신하여 사용자의 도안 작업을 보조할 수 있도록 안내합니다.

## 지원 범위

- **원격 MCP 연동**: Streamable HTTP 프로토콜 및 OAuth 2.1 Dynamic Client Registration(DCR)을 통한 안전한 연결
- **도안 데이터 조회**: KNITFORM MCP 엔드포인트를 통해 제공되는 도안 데이터 조회 (`mcp:read` 스코프)
- **차트 및 표기 지원**: KNITFORM의 표준 SVG 기호 및 뜨개 표기 규칙 준수

## 주의사항

- 사용자의 기존 도안 및 웹서비스 데이터는 안전하게 보호되어야 합니다.
- 인증은 OAuth DCR 흐름으로 처리되며, API 키나 비밀번호를 별도로 입력하거나 코드에 저장하지 않습니다.
