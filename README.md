# FutureFinder

**경제·진로 고민을 함께 해결하며 사회로 나아가는 첫걸음을 돕는 청년 맞춤형 커리어 가이드 플랫폼**

2025 시즌톤 85팀의 Flutter 프론트엔드 프로젝트입니다. 금융·자산, 주택 청약, 일자리 정보를 한곳에 모으고 경제 용어 검색과 사용자별 정보 화면을 제공합니다.

[백엔드 저장소](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_BE)

## 주요 기능

| 영역 | 구현 내용 |
| --- | --- |
| 회원·인증 | 단계별 회원가입, 로그인 API 연동, 토큰·사용자 정보 저장, 홈 진입 시 인증 상태 및 토큰 만료 처리 |
| 홈 | 사용자 정보 표시, 금융·청약·일자리 화면 이동, 경제 용어 검색 진입 |
| 경제 용어 검색 | 검색 API 연동, 용어 설명 표시, 긴 검색 결과 스크롤 |
| 금융·자산 | 자산 목록·등록·인증 화면, 자산 모델과 유형별 이미지 매핑, 자산 조회 API 연결 코드 |
| 청약 | 청약통장·관심 지역·등록·인증·챗봇 화면 |
| 일자리 | 학력·활동 입력 온보딩, 추천 공고·대외활동 화면 및 조회 Repository |
| 공통 UI | 하단 탭 탐색, 북마크·설정 화면, 데이터 로딩 오버레이 |

해커톤 당시의 구현 상태를 담고 있습니다. 금융·청약·북마크·설정과 일부 추천 화면에는 더미 데이터가 포함되어 있습니다. 청약 챗봇은 고정 응답을 표시하는 UI이며, 자산 API 연동은 진행 중인 상태입니다. 일자리 온보딩은 입력값을 임시 보관하고 API 실패 시 더미 데이터를 사용하는 로직을 포함합니다.

## 주요 기여

Flutter 화면 구현, 데이터 계층 구성, 주요 API 연동과 웹 배포 자동화를 담당했습니다.

| 영역 | 주요 작업 | 관련 PR |
| --- | --- | --- |
| 앱 구조·데이터 계층 | MVVM 구조, Provider 의존성 주입, 공통 API 클라이언트·응답 DTO·예외 정의, 플랫폼별 저장소 인터페이스 구성 | [#1](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/1) |
| 화면·탐색 | 홈·금융·청약·일자리·설정 화면 레이아웃, 로그인·스플래시 화면, go_router 기반 화면 전환과 탭 탐색 구성 | [#9](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/9), [#10](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/10), [#11](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/11) |
| 인증 연동 | 로그인·회원가입 API 연결, 로그인 후 사용자 정보 조회, 홈 진입 시 미인증·토큰 만료 예외 처리 | [#16](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/16), [#17](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/17), [#18](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/18), [#24](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/24) |
| 검색·로딩 | 경제 용어 검색 API 및 결과 화면, 북마크 화면, EasyLoading 오버레이와 검색 결과 스크롤 처리 | [#19](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/19), [#20](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/20), [#21](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/21) |
| 금융·청약 | 자산 연결·청약 챗봇 레이아웃, 자산 모델·이미지 매핑 및 자산 API 연동 작업 | [#14](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/14), [#15](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/15), [#23](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/23), [#24](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/24) |
| 웹 배포 | GitHub Actions를 통한 Flutter 웹 빌드, Nginx Docker 이미지 및 EC2 배포 워크플로 구성·수정 | [#1](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/1), [#6](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/6), [#7](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/7), [#8](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pull/8) |

전체 개발 내역은 [PR 목록](https://github.com/9oormthon-univ/2025_SEASONTHON_TEAM_85_FE/pulls?q=is%3Apr)에서 확인할 수 있습니다.

## 기술 스택

| 구분 | 기술 |
| --- | --- |
| 언어·프레임워크 | Dart, Flutter — 배포 워크플로 기준 Flutter 3.35.3, Dart SDK 제약 ^3.8.0 |
| 상태 관리·구조 | Provider, ChangeNotifier, MVVM |
| 라우팅 | go_router, StatefulShellRoute |
| 통신 | http, Dio, 공통 응답 DTO·API 예외 처리 |
| 저장소 | 모바일: flutter_secure_storage / 웹: shared_preferences |
| UI | Material, flutter_easyloading, intl |
| 배포 | GitHub Actions, Docker, Nginx, AWS EC2 |

## 프로젝트 구조

```text
lib/
├── main.dart            # 앱 진입점·테마·API 주소
├── di/                  # Provider 의존성 주입
├── data/                # API 클라이언트·플랫폼별 저장소
├── dto/                 # 인증·공통 응답 DTO
├── exception/           # API 예외
├── model/               # 사용자·자산·검색·일자리 모델
├── repository/          # 인증·검색·자산·일자리 API 접근
├── viewmodel/           # 화면 상태·데이터 처리
├── router/              # go_router 설정
├── mixin/               # 공통 로딩 처리
└── view/                # 홈·금융·청약·일자리·회원·설정 화면
assets/images/           # 로고·유형별 아이콘
web/                     # 웹 진입 파일·스플래시
.github/workflows/       # 웹 빌드·배포 자동화
```

View → ViewModel → Repository → ApiClient 순서로 화면 상태와 API 접근을 나누고, Provider로 의존성을 전달합니다. 토큰 저장은 웹에서 SharedPreferences, 모바일에서 FlutterSecureStorage를 사용합니다.

## 로컬 실행

배포 환경과 맞추려면 Flutter 3.35.3을 사용합니다. 웹 실행에는 Chrome이 필요하며, 모바일 실행에는 해당 플랫폼의 SDK와 에뮬레이터 또는 실기기가 필요합니다.

```bash
flutter pub get
flutter run -d chrome
```

연결 가능한 기기는 `flutter devices`로 확인할 수 있습니다.

### API 주소 설정

현재 API 주소는 [lib/main.dart](lib/main.dart)의 `getProviders('http://15.164.172.236/api')`로 지정되어 있습니다. 로컬 백엔드에 연결하려면 해당 인자를 실행 환경에 맞게 변경합니다.

| 실행 환경 | 백엔드 주소 예시 |
| --- | --- |
| 같은 PC의 Chrome | `http://localhost:8080/api` |
| Android 기본 에뮬레이터 | `http://10.0.2.2:8080/api` |
| 실기기 | `http://<개발 PC의 LAN IP>:8080/api` |

위 주소는 백엔드가 8080 포트와 `/api` 접두사를 사용할 때의 예시입니다. 현재 `.env`나 `--dart-define`을 통한 API 주소 주입은 구현되어 있지 않습니다. 웹에서 다른 출처의 백엔드를 호출하려면 서버의 CORS 설정도 필요합니다.

## 빌드 및 확인

```bash
flutter analyze
flutter build web
```

웹 빌드 결과물은 `build/web/`에 생성됩니다. 저장소에는 플랫폼별 프로젝트 디렉터리가 포함되어 있지만, 현재 자동 배포 대상은 웹입니다.

[test/widget_test.dart](test/widget_test.dart)는 Flutter 기본 카운터 테스트 내용이 남아 있어 현재 앱 화면과 맞지 않습니다. 서비스 동작을 검증하는 테스트로 사용하려면 수정이 필요합니다.

## 웹 배포

[배포 워크플로](.github/workflows/deploy-main.yml)는 `main` push 시 다음 작업을 수행합니다.

1. Flutter 3.35.3 설치 및 패키지 복원
2. `flutter build web` 실행
3. 웹 결과물을 포함한 Nginx Docker 이미지 빌드·푸시
4. SSH로 EC2에 접속해 `/opt/futurefinder`에서 Docker Compose 배포

[Dockerfile](Dockerfile)은 빌드된 `build/web/` 파일을 Nginx에 복사합니다. Docker 이미지를 로컬에서 만들 때도 Flutter 웹 빌드를 먼저 실행해야 합니다.

배포에는 `futurefinder_flutter` GitHub Environment와 `IMAGE_NAME`, `DOCKER_USERNAME`, `DOCKER_PASSWORD`, `EC2_HOST`, `EC2_USERNAME`, `EC2_SSH_KEY` Secrets가 필요합니다. 서버의 Docker Compose 구성은 별도로 준비해야 합니다. 현재 코드에 지정된 API 서버의 운영 여부는 확인하지 않았습니다.
