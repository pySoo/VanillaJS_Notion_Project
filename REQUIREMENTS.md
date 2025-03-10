## 기본 요구사항

바닐라 JS만을 이용해 노션을 클로닝합니다.

기본적인 레이아웃은 노션과 같으며, 스타일링, 컬러값 등은 원하는대로 커스텀합니다.

글 단위를 Document라고 합니다. Document는 Document 여러개를 포함할 수 있습니다.

- [x] 화면 좌측에 Root Documents를 불러오는 API를 통해 루트 Documents를 렌더링합니다.

- [x] 해당 Root Document에 하위 Document가 있는 경우, 해당 Document 아래에 트리 형태로 렌더링 합니다. (무한 documents는 추가로 해야함)

- [x] Root Document를 클릭하면 오른쪽 편집기 영역에 해당 Document의 Content를 렌더링합니다.

- [x] Document Tree에서 각 Document 우측에는 + 버튼이 있습니다. 해당 버튼을 클릭하면, 클릭한 Document의 하위 Document로 새 Document를 생성하고 편집화면으로 넘깁니다.

- [x] 편집기에는 기본적으로 저장 버튼이 없습니다. Document Save API를 이용해 지속적으로 서버에 저장되도록 합니다.

- [x] History API를 이용해 SPA 형태로 만듭니다.

- [x] 루트 URL 접속 시엔 별다른 편집기 선택이 안 된 상태입니다.

- [x] /documents/{documentId} 로 접속시, 해당 Document 의 content를 불러와 편집기에 로딩합니다.

## 보너스 요구사항

- [x] 편집기 최하단에는 현재 편집 중인 Document의 하위 Document 링크를 렌더링하도록 추가합니다.

그외 개선하거나 구현했으면 좋겠다는 부분이 있으면 적극적으로 구현해봅니다!
