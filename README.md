# 알루미늄 연결 압출품 — REV B 재검토와 REV C 제안

제품 형상은 그대로 두고 흰 연결부의 위치·형태만 변경한 검토 자료입니다. **완전 파단이나 금형 제작을 승인한 도면이 아닙니다.**

## 최신 자료 다운로드

- **[보고서·도면·움직임 GIF·계산 자료 전체 ZIP](https://github.com/dltkdghk1103-hue/-/raw/refs/heads/main/downloads/revB_revC_complete_download.zip)**
- [REV B 재검토 및 REV C 추천 보고서 PDF](https://github.com/dltkdghk1103-hue/-/raw/refs/heads/main/downloads/revB_revC_review_KO.pdf)
- [REV C 연결부 수정 DXF](https://github.com/dltkdghk1103-hue/-/raw/refs/heads/main/downloads/bridge_relocated_revC_CONCEPT.dxf)
- [REV C 도면 PDF](https://github.com/dltkdghk1103-hue/-/raw/refs/heads/main/downloads/bridge_relocated_revC_CONCEPT.pdf)
- [양끝 완전 분리 후 조건부 낙하 비교 GIF](https://github.com/dltkdghk1103-hue/-/raw/refs/heads/main/downloads/conditional_drop_revB_revC.gif)
- [입력·계산 코드·결과 ZIP](https://github.com/dltkdghk1103-hue/-/raw/refs/heads/main/downloads/review_results_and_sources.zip)
- [보고서 웹에서 읽기](downloads/revB_revC_review_KO.md)
- [제품 형상 보존 기록](downloads/geometry_preservation.json) · [접촉 계산 검산](downloads/trajectory_numerical_checks.json)

기존 `report_and_modified_drawings.zip`과 `extrusion_analysis_report_KO.pdf` 주소도 최신 자료로 갱신했습니다. 비공개 저장소이면 접근 가능한 GitHub 계정으로 로그인한 뒤 파일 화면의 **Download raw file** 버튼을 이용하세요.

## 이번 결론

- **REV B:** 정밀 접촉 계산에서 상단 입구에 남았습니다. 거친 계산의 일부 낙하 결과는 시간 간격을 줄이자 바뀌었으므로 안정 낙하의 근거로 쓰지 않았습니다.
- **REV C:** 흰 연결부를 기존 초록 내벽과 노란 판 밑면 사이로 이동했습니다. 초록 목 0.35 mm, 노란 목 0.25 mm, 몸통 약 0.65 mm. 노란 목이 조금 먼저 약해지고, 내려오는 판이 남은 초록 목을 계속 누르는 배치를 우선 추천합니다.
- **내부 진입:** 두 목이 이미 완전히 끊어진 조건에서 기본 9개와 초기 반동 12개 모두 내부 바닥 영역에 도달했습니다. 이 개수는 작업 성공률이 아닙니다. 일부 기본 조건에서 움직임이 남았고 최종 위치도 달라져, 모든 조건의 안정 정지까지 확인한 것은 아닙니다.
- **두 번째 목:** 초록 목이 먼저 끊어지면 기존 경사벽 접촉이 있어야 남은 노란 목에 추가 힘이 전달됩니다. 균열 틈·미끄러짐에 따라 접촉이 없어질 수 있어, 어느 순서든 깨끗하게 끊어진다는 보장은 없습니다.
- **6 m / 사람 힘:** 100 mm 환산값은 손 접촉 폭과 같지 않습니다. 판 휨을 제외하고 6 m 전체가 함께 내려가는 모델은 손 압력만으로 전 길이 동시 분리를 지지하지 않습니다. 고무망치의 실제 파단과 길이 방향 순차 균열은 검증하지 않았습니다.

![연결부 위치·형태 변경](downloads/revC_geometry.png)

## 제품 형상과 모델의 범위

원본 노란색·초록색 제품 엔티티 4개의 좌표, 원호 bulge, 폭, 열린/닫힌 상태를 DXF 저장 후 비교했습니다. 모두 동일합니다. 제품에 턱·홈·가이드·돌출부를 추가하지 않았습니다. 원래 목 끝면의 폐곡선 표시와 새 연결부의 재료 접속선을 구분해서 읽어야 하며, DXF는 금형 와이어 가공용 윤곽도가 아닙니다.

보고서는 탄성 목 단면 비교, 한 목 제거 후 하중 전달 근사, 양끝 분리 후 강체 접촉 계산을 구분합니다. 균열 생성부터 최종 낙하까지 이어지는 손상 해석이 아닙니다. 무고정 제품에 대한 편심 타격·기울어짐, 고온 소성, 실제 버, 6 m 비틀림·파단 전파, 다이 유동·강도는 검증하지 않았습니다.

## 이전 자료

[REV B 도면 DXF](downloads/modified_bridge_only_revB_CONCEPT.dxf)와 [이전 정정 보고서](downloads/corrected_report_revB_KO.pdf)는 이력용입니다. REV B의 최신 낙하 판단은 위 최신 보고서를 보세요.

**REV A는 철회 상태입니다.** 제품에 안내 턱을 추가하고 제품 목 주변을 변경한 이전 안은 형상 보존과 포개짐 조건에 맞지 않았습니다. 현재 파일 목록에 REV A 도면은 없으며, 이미 받은 REV A는 사용 대상이 아닙니다.
