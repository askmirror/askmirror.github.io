# MirrorMirror — AI Agents Deserve the Truth

> *"Mirror, mirror, on the wall — show me what this API really calls."*

**MirrorMirror**는 AI 코딩 에이전트를 위한 inspection MCP(Model Context Protocol) 서버 컬렉션입니다.  
API, 데이터베이스, 환경, 의존성, 설정 — 추측 대신 사실을 비춰줍니다.

🌐 **Website:** [https://askmirror.net](https://askmirror.net)

---

## The Problem

AI 코딩 에이전트는 학습 데이터에 기반하여 API를 "기억"합니다.  
하지만 그 기억은 종종 오래되었거나, 존재하지 않는 메서드를 포함합니다.  
결과는 컴파일 오류, 런타임 예외, 그리고 디버깅에 낭비되는 시간입니다.

MirrorMirror는 AI 에이전트가 추측하는 모든 곳에 거울을 놓습니다.

---

## Products

### 🪞 HandMirrorMcp — .NET Assembly Inspector *(Open Source)*

.NET 어셈블리와 NuGet 패키지를 실시간으로 inspection합니다.  
타입, 메서드, 네이티브 인터롭, 프로젝트 구조, 빌드 에러까지 — AI 에이전트가 정확한 코드를 생성할 수 있도록 합니다.

- **Free (Open Source):** 어셈블리/타입 inspection, NuGet 패키지 분석, 보안 취약점 조회, 네이티브 인터롭 분석, 프로젝트/솔루션 분석, 빌드 에러 설명, 설정 파일 분석, 시스템 및 .NET 런타임 정보
- **Pro:** 다중 어셈블리 비교, 크로스 어셈블리 타입 의존 관계 그래프, API breaking change 감지, .nupkg 심층 분석, 솔루션 전체 일괄 분석 리포트

📦 [NuGet](https://www.nuget.org/packages/HandMirrorMcp) · 🔗 [GitHub](https://github.com/rkttu/HandMirrorMcp)

### Coming Soon

| Product | Description |
|---|---|
| **SqlMirrorMcp** | Database Schema Inspector — 데이터베이스의 실제 스키마 구조를 비춥니다 |
| **OpsMirrorMcp** | System Environment Inspector — 코드가 실행될 환경의 실제 상태를 비춥니다 |
| **PkgMirrorMcp** | Package & Dependency Inspector — 프로젝트에 실제 설치된 의존성의 진실을 비춥니다 |
| **NetMirrorMcp** | Network & Endpoint Inspector — API 엔드포인트의 실제 응답 구조를 비춥니다 |
| **ConfMirrorMcp** | Configuration Inspector — 설정 파일의 실제 구조와 현재 값을 비춥니다 |
| **SchemaMirrorMcp** | Data Format Inspector — 데이터 직렬화 스키마의 실제 구조를 비춥니다 |
| **DocMirrorMcp** | Documentation Inspector — 코드와 문서 사이의 불일치를 비춥니다 |

---

## Philosophy

- **Inspect, Don't Guess** — 학습 데이터에 의존하지 않습니다. 실제 바이너리, 실제 스키마, 실제 시스템 상태를 직접 읽습니다.
- **The Mirror Never Lies** — 거울은 아첨하지 않습니다. API가 deprecated되었으면 deprecated라고 말하고, 메서드가 없으면 없다고 말합니다.
- **Local First, Always** — 모든 inspection은 로컬에서 수행됩니다. 코드가 외부로 전송되지 않습니다. 오프라인에서도 동작합니다.

---

## Quick Start (HandMirrorMcp)

```bash
# Install as .NET global tool
dotnet tool install -g HandMirrorMcp
```

`claude_desktop_config.json`에 추가:

```json
{
  "mcpServers": {
    "handmirror": {
      "command": "HandMirrorMcp"
    }
  }
}
```

👉 [Full Setup Guide](https://github.com/rkttu/HandMirrorMcp#readme)

---

## Repository Structure

```
docs/
  index.html    # MirrorMirror landing page (https://askmirror.net)
```

이 리포지터리는 MirrorMirror 제품 스위트의 랜딩 페이지를 호스팅하는 GitHub Pages 사이트입니다.

---

## Links

- 🌐 Website: [askmirror.net](https://askmirror.net)
- 📦 HandMirrorMcp NuGet: [nuget.org/packages/HandMirrorMcp](https://www.nuget.org/packages/HandMirrorMcp)
- 🔗 HandMirrorMcp GitHub: [github.com/rkttu/HandMirrorMcp](https://github.com/rkttu/HandMirrorMcp)
- 📰 Newsletter: [/dev/write](https://letter.rkttu.com)
- 💬 Forum: [forum.dotnetdev.kr](https://forum.dotnetdev.kr)

---

## License

© 2025 [rkttu.com](https://rkttu.com) · Built by [Jung Hyun, Ryu](https://github.com/rkttu)
