### CSS 작동방식

* 브라우저는 HTML (예: 네트워크에서 HTML 을 수신) 을 로드합니다.

* HTML 을 DOM (Document Object Model) 로 변환합니다. DOM 은 컴퓨터 메모리의 문서를 나타냅니다. DOM 은 다음 섹션에서 좀 더 자세히 설명됩니다.

* 그런 다음 브라우저는 포함된 이미지 및 비디오와 같은 HTML 문서에 연결된 대부분의 리소스와 연결된 CSS 를 가져옵니다! JavaScript 는 작업에서 나중에 처리되므로 더 간단하게 하기위해 여기에서는 다루지 않습니다.

* 브라우저는 가져온 CSS 를 구문 분석하고 선택자 유형별로 다른 규칙을 다른 "buckets" 으로 정렬합니다. 예: 요소, class, ID 등 찾은 선택자를 기반으로 DOM 의 어느 노드에 어떤 규칙을 적용해야 하는지 결정하고, 필요에 따라 스타일을 첨부합니다 (이 중간 단계를 render tree 라고 합니다).

* render tree 는 규칙이 적용된 후에 표시되어야 하는 구조로 배치됩니다.

* 페이지의 시각적 표시가 화면에 표시됩니다 (이 단계를 painting 이라고 함)

<img src="https://mdn.mozillademos.org/files/11781/rendering.svg">