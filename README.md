# Smartway_LineInspect

# Commit Convention Guide

## Commit Message Structure

```
[type] scope: subject

body (상세 내용)
- 변경사항 1
- 변경사항 2

footer (부가 정보)
Performance: xxx
Test: xxx
Reference: xxx
```

## Type 정의

### Vision 관련 [vision-*]
- vision-param: 파라미터 설정 폼 관련
- vision-roi: ROI 설정 창 관련
- vision-test: 테스트 창 관련
- vision-camera: 카메라 클래스 관련
- vision-inspect: 검사 클래스 관련
- vision-core: 비전 메인 클래스 관련

### Motion 관련 [motion-*]
- motion-thread: 상태 쓰레드 관리 관련
- motion-group: 그룹 관리 클래스 관련
- motion-test: 테스트 창 관련
- motion-control: 메인 컨트롤 창 관련
- motion-param: 파라미터 설정 관련

### DIO 관련 [io-*]
- io-group: 그룹 관리 클래스 관련
- io-control: 메인 컨트롤 창 관련

### 시퀀스 관련 [seq-*]
- seq-core: 시퀀스 관리 클래스 관련
- seq-monitor: 모니터링 창 관련

### 시리얼 통신 관련 [serial-*]
- serial-core: 시리얼 매니저 클래스 관련
- serial-control: 통신 컨트롤 창 관련

### 설정 관련 [config-*]
- config-param: 프로그램 설정 파라미터 관련
- config-message: 메시지 박스 관련
- config-log: 로그 창 관련

### 메인 관련 [main-*]
- main-draw: 그리기 관리 클래스 관련
- main-init: 초기화 클래스 관련
- main-handler: 핸들러 컨트롤 클래스 관련

## Commit Message 예시

```
[vision-roi]: ROI 다중 선택 기능 추가

- 마우스 드래그로 다중 ROI 선택 가능
- ROI 그룹 저장/불러오기 기능 추가
- ROI 속성 일괄 수정 기능 구현

Performance: ROI 설정 시간 30% 단축
Test: 다중 ROI 100개 생성/수정 테스트 완료
```

```
[motion-thread]: 모터 상태 감시 최적화

- 쓰레드 업데이트 주기 조정 (100ms → 50ms)
- 비정상 상태 감지 로직 개선
- 메모리 사용량 최적화

Stability: CPU 사용률 5% 감소
Safety: 비상정지 반응속도 향상
```

## Footer 키워드 가이드
- Performance: 성능 개선 수치
- Accuracy: 정확도 변화
- Safety: 안전 검증 결과
- Test: 테스트 결과/범위
- Reference: 참고한 규격/문서
- Related: 관련된 이슈/문서

## control
- servo=control 기능 추가