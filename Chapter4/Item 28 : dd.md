# Item 28: API 안전성 명시

## 프로그래밍에서 표준화된 API를 선호하는 이유

### 1. API 변경으로 발생되는 문제점

API 변경이 코드의 수동 업데이트를 필요로 하며, 이는 다음과 같은 경우에 문제가 될 수 있습니다.

- API에 의존하는 요소가 많은 경우
- 익숙하지 않은 프로젝트에 API를 사용한 경우

공개 라이브러리를 사용하는 경우 개발자들이 직접 라이브러리를 수정할 수 없으므로, API를 사용하는 코드를 직접 수정해야 합니다.
이러한 수정들이 코드 전반에 큰 변경을 요구하게 되어 개발자들은 오래된 라이브러리 버전을 계속해서 사용하게 되는 경우가 빈번합니다.

개발자들이 오래된 라이브러리를 계속해서 사용하게 되는 경우 다음과 같은 문제가 발생될 수 있습니다.

- 라이브러리를 업데이트 하는것에 더욱 더 어려움이 생깁니다.
- 높은 버전의 라이브러리에서 제공되는 기능을 놓칠 수 있습니다.
- 오래된 라이브러리는 지원이 중단되거나 완전히 작동을 멈출 수 있습니다.

따라서 새로운 안정된 라이브러리 버전을 사용하는것을 두려워하는 개발자들이 있는 상황은 좋은 상황이 아닙니다.

### 2. API 변경사항의 새로운 학습과 보안 이슈

새로운 API 학습은 개발자들에게 부담을 주며, 새로운 지식으로 갱신하는 것을 회피하는 경향이 있습니다.
이러한 점은 좋지 않으며, 오래된 지식은 결국 보안 문제로 이어질 수 있습니다.