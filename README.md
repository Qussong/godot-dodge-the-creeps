# godot-dodge-the-creeps

Godot 공식 튜토리얼 **["Your first 2D game — Dodge the Creeps"](https://docs.godotengine.org/en/stable/getting_started/first_2d_game/index.html)** 를 따라 만드는 학습용 프로젝트입니다.

## 개요

하늘에서 떨어지는 적(creeps)을 피하며 최대한 오래 버티는 2D 아케이드 게임입니다.

- **엔진:** Godot 4.7 (Forward Plus)
- **언어:** GDScript
- **목적:** Godot 입문 — 씬/노드 구조, 시그널, 입력 처리, 스폰 로직, HUD 학습

## 개발 환경

| 항목 | 값 |
|------|-----|
| Godot | 4.7 |
| 렌더러 | Forward Plus |
| 물리 | Jolt Physics |
| Windows 드라이버 | Direct3D 12 |

## 조작 방법

- 이동: 방향키 / WASD
- 게임 시작: Enter 키 또는 Start 버튼 클릭
- 게임패드(컨트롤러) 입력 지원

## 실행 방법

### 직접 플레이 (빌드된 파일)

[Releases](https://github.com/Qussong/godot-dodge-the-creeps/releases) 페이지에서 최신 버전을 다운로드해 압축을 풀고 실행 파일을 바로 실행할 수 있습니다.

### 에디터에서 실행

1. [Godot 4.7](https://godotengine.org/download) 이상 설치
2. 저장소 클론
   ```bash
   git clone https://github.com/Qussong/godot-dodge-the-creeps.git
   ```
3. Godot에서 `project.godot` 열기 → `F5`

## 프로젝트 구조

```
.
├── art/                # 스프라이트, 효과음, 배경 음악
├── fonts/              # Xolonium 폰트 (HUD용)
├── player.tscn/.gd     # 플레이어 씬 · 이동/애니메이션 처리
├── mob.tscn/.gd        # 몹 씬 · 랜덤 스폰/이동 처리
├── hud.tscn/.gd        # HUD · 점수/메시지/시작 버튼
├── main.tscn/.gd       # 메인 씬 · 게임 루프, 스폰 타이머
├── export_presets.cfg  # 내보내기(export) 설정
├── icon.svg            # 프로젝트 아이콘
└── project.godot       # 프로젝트 설정
```

## 진행 상황

- [x] 프로젝트 생성 및 에셋 임포트
- [x] Player 씬 (이동 · 애니메이션 · 화면 경계)
- [x] Mob 씬 (랜덤 스폰 · 이동)
- [x] Main 씬 (게임 루프 · 스폰 타이머)
- [x] HUD (점수 · 메시지 · 시작 버튼)
- [x] 배경 음악 및 효과음
- [x] 마무리 (배경, 애니메이션 정리)
- [x] Windows 빌드 내보내기

## 라이선스

- 코드: 학습용 개인 프로젝트
- 에셋: Godot 예제 에셋 (`art/`), 폰트는 `fonts/LICENSE.txt` 참고
