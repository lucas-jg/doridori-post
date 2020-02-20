## 시작
Javascript를 사용하게 된지 벌써 1년이 지나가고 있습니다.

지금까지 일정에 치여 바쁘게 업무만 진행하다 보니 처음 자바스크립트를 시작했을 당시 대충 책 뒤져본 내용 그대로 발전없이 어려운 길을 가고 있다는 생각이 들었죠.
그래서 자바스크립트를 사용하여 알고리즘 문제를 풀고, ES6 문법과 표준에 대해 조금더 익숙해지려고 합니다. 

**공부한 내용과 피드백 받은 내용들에 대해 공유하기 위해 하나하나 적어가보려고 합니다.**

자바스크립트를 공부하기 위해 [Exercism](https://exercism.io)이라는 서비스를 사용하고 있으며 외국인 멘토들이 제가 작성한 코드를 보고 피드백을 주는 사이트입니다. 관심있는 사람은 가입해서 멘토링을 진행해보세요. 문제를 풀고 내가 의도한 내용과 질문을 등록하면 맨토들이 코드와 질문을 보고 피드백을 줍니다.

**앞으로 제가 맨토가 되어 Exercism에서 멘토링을 진행하는 그날까지 이 시리즈는 계속 됩니다.
(영어 공부에도 도움이 됩니다 🤭🤭🤭🤭)**

분명 책에서 보고 알고 있던 문법과 방식이지만, 실제로 사용하지 않고 예전 습관 그대로 손이 반응하여 치는 코드들이 많다는 것을 느끼고 있습니다. 
부족함이 느껴지지만 제 자신의 발전을 위해 그리고 혹시나 저와 같은 상황에 놓인 또 다른 누군가에게 도움이 되기를 바라며 🤟🤟

너무나 쉬운 문제이지만 최신 동향을 따라가지 못한 코드도 있습니다. 최신 동향이 무조건 답은 아니라고 생각하지만, 제대로 알고 판단해도 늦지 않겠죠? 일단 무작정 시작해 봅시다.

서론은 이정도로 하고 앞으로 이어지는 시리즈에는 문제와 풀이의 비중을 높혀 작성 할 것에요. 
다들 화이팅입니다.

---

### 문제

Two-fer or 2-fer is short for two for one. One for you and one for me.
Given a name, return a string with the message:

> One for X, one for me.

Where X is the given name.
However, if the name is missing, return the string:

> One for you, one for me.

Here are some examples:
```
Name	   String to return
Alice	  One for Alice, one for me.
Bob	    One for Bob, one for me.
           One for you, one for me.
Zaphod	 One for Zaphod, one for me.
```

### 첫번째 코드
```javascript
export const twoFer = name => {
  return `One for ${!!name ? name : "you"}, one for me.`;
};
```
**사용된 관련 문법**
* [Conditional operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)
* [Template Literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals) 

**피드백**
I invite you to check out the following features and try to incorporate them to your solution:
 * [default function parameters](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Default_parameters)
 * [concise function body](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions#Function_body)

### 최종 코드
```javascript
export const twoFer = (name = "you") => `One for ${name}, one for me.`;
```
**추가 의견**
첫번째 코드와 최종 코드 모두 같은 결과를 내는 코드입니다. 하지만 지금 집중하는 것은 최신 동향의 ES6 문법을 공부하는 것이기 때문에 앞으로의 코드들은 최대한 적용해 보려고합니다.
이 글을 읽고 있다면 링크를 걸어둔 Javascript Docs를 꼭 확인해주세요.

----

**앞으로 제가 맨토가 되어 Exercism에서 멘토링을 진행하는 그날까지 이 시리즈는 계속 됩니다.**

### 자료
* [Exercism](https://exercism.io)
* [MDN web docs](https://developer.mozilla.org/en-US/)
* Photo by Joshua Aragon on Unsplash
