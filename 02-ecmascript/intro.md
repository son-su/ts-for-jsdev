---
description: 2장에선 타입스크립트의 기반이 되는 언어 ECMAScript 최신 명세에 추가된 여러 유용한 기능들을 살펴본다.
---

# 2.0 ECMAScript

앞서 언급했듯, 타입스크립트는 자바스크립트의 상위집합\(superset\)이다. **모든 자바스크립트 코드는 곧 적법한 타입스크립트 코드이다**. 때문에 타입스크립트 프로그래머는 자바스크립트 관련 지식을 십분 활용할 수 있는 한편, 자바스크립트 언어의 한계 또한 안고 가야 한다. 어느 쪽에 초점을 맞추든, 타입스크립트 프로그래밍을 위해서 자바스크립트 언어에 관한 지식은 필수적이다. 

**타입스크립트는 최신 자바스크립트 표준의 명세를 대부분 지원한다.** 최신 자바스크립트 명세에 익숙해지는 과정은 실력 있는 타입스크립트 프로그래머로 나아가기 위한 첫걸음이나 다름 없다. 이 책은 자바스크립트 경험을 가진 독자를 대상으로 한다. 그럼에도 ECMAScript 2015 이후의 표준을 비롯해 상대적으로 최근 들어 추가된 기능에 아직 익숙해지지 않은 독자가 꽤 있을 것이다. 

2장에서는 보다 나은 타입스크립트 프로그래머가 되기 위해 알아야 할 최신 자바스크립트 기능 중 특히 자주 쓰일 일부를 소개한다. ES5에서 ES7에 이르기까지의 방대한 변경 사항을 전부 담는 것은 이 책의 목표가 아니므로, **이 장에서는 새로운 스펙 중 상대적으로 자주 쓰이는 기능에 대해서만 다룬다**.

{% hint style="info" %}
이 장의 코드 예제는 모두 [strict mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode)에서 실행될 것을 가정하고 있다.
{% endhint %}

{% hint style="info" %}
2장을 적으며 니콜라스 자카스\(Nicholas C. Zakas\)가 저술하고 국내에서는 인사이트 출판사에서 번역해 출판한 [『모던 자바스크립트 : 예제로 배우는 ECMAScript 6 핵심 기능』](http://www.insightbook.co.kr/book/programming-insight/%EB%AA%A8%EB%8D%98-%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8)의 내용으로부터 많은 도움을 받았다. 여기 소개된 기능을 비롯해 ECMAScript 6에 추가된 다양한 기능에 대한 더 자세한 설명을 원하는 독자에게는 해당 서적을 추천한다.
{% endhint %}

**만약 이미 최신 ECMAScript에 익숙한 독자라면 2장을 건너뛰고 바로 3장으로 가도 무방하다**. 또한 이 장에서는 독자가 ECMAScript, TC39 등의 자바스크립트 언어 표준에 관한 기본적인 지식을 갖고 있을 것이라 가정한다. 만약 그렇지 않다면 아래 링크를 통해 _부록 II : 자바스크립트 언어 생태계_를 참조하라.

{% page-ref page="../appendix-ii-js-ecosystem/ecmascript-tc39.md" %}
