## 무엇을
<!-- 변경 내용 요약 -->

## 왜
<!-- 배경. 이슈가 있으면 아래 Closes에 번호 -->

## 영향 범위
<!-- 해당하는 것에 x -->
- [ ] `control/` 제어·추정 로직
- [ ] `plant/` 차량 모델
- [ ] `input/` 입력 노드
- [ ] `firmware/` STM32
- [ ] `hmi/` 모니터링
- [ ] `dbc/` CAN 정의 ⚠️ 전 노드 영향
- [ ] `scenarios/` / `tools/` / `tests/`
- [ ] `docs/`

## 확인
- [ ] 빌드 통과
- [ ] 단위테스트 통과 (`control/` 변경 시 필수)
- [ ] 단위 SI 준수 (내부 m/s·m·N·kg, 표시에서만 km/h)
- [ ] `control_step()` 순수성 유지 — 전역변수·하드웨어 의존 없음
- [ ] DBC 변경 시: 송신·수신 양쪽 노드 모두 반영
- [ ] 설계 결정이 바뀌었다면 `docs/decisions.md` 갱신

## 검증 방법
<!-- 어떻게 확인했는지. 예: vcan0에서 candump로 0x200 주기 확인 -->

Closes #
