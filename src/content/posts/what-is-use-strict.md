---
title: 엄격 모드(strict mode)는 무엇인가?
category: javascript
date: 2023-02-07T12:46:11+09:00
---

오랫동안 자바스크립트는 호환성 이슈 없이 발전해 왔습니다. 기존의 기능을 변경하지 않으면서 새로운 기능을 추가해 왔습니다.

이것은 기존의 코드를 깰 일이 없다는 이점을 가졌습니다. 그런데, 자바스크립트를 고안한 사람들의 실수나 불완전한 결정이 언어 안에 영원히 남는다는 불리한 점이 있었습니다.

이런 상황은 ECMAScript5(ES5)가 등장한 2009년까지 지속되었습니다. ES5에서는 새로운 기능이 추가되었고, 몇몇 기존 기능이 변경되었습니다. 예전 코드의 동작을 보장하기 위해서 이러한 변경 사항이 기본적으로는 해제되어 있도록 설계되었습니다. 이 변경 사항을 적용하기 위해서는 `"use strict"` 라는 특별한 지시자를 통해서 명시적으로 활성화할 필요가 있습니다.

`"use strict"` 혹은 `'use strict'` 지시자를 스크립트의 최상단에 위치시키면, 그 스크립트 전체는 모던한 방식으로 동작합니다.

예를 들면 다음과 같습니다.

```js
"use strict";

// 여기에 작성되는 코드는 모던한 방식으로 동작합니다.
```

모던 자바스크립트는 고급 언어 구조인 클래스와 모듈 기능을 지원합니다. 이 둘을 사용하고 있다면 엄격 모드는 자동으로 활성화됩니다. 그래서 그런 경우에는 `"use strict"` 지시자를 생략해도 됩니다.

### Resources

- https://javascript.info/strict-mode
