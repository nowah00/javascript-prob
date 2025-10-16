# Day01 자바스크립트 문제

---
1. 다음 중 재할당이 불가능한 선언은?

A) `var a = 1`  B) `let a = 1`  C) `const a = 1`

→ C

---
**2.** 아래 코드의 출력결과는?

```jsx
console.log(x);
var x = 10;

// 정답
> 10
```

---
**3.** 아래 코드에서 에러가 나는 줄은? 이유는?

```jsx
console.log(y);
let y = 3;

// 정답
// y가 만들어지기 전에 출력을 먼저 했기 때문이다.
```

---
**4.** `const obj = { n: 1 };`

    obj 객체의 속성 n 의 값을 2로 변경하세요. 

→ `obj.n = 2;`

---
**5.** 다음 중 올바른 식별자(변수명)가 아닌 것은?

A) `_count` B) `$value` C) `2nd` D) `camelCase`

→ C (숫자로 시작하면 안됌)

---
**6.** 다음 코드의 결과?

```jsx
let a = 1;
a = a + 2;
console.log(a);

//정답
> 3
```

---
**7.** 템플릿 리터럴로 “Hello, JS!”를 만들 올바른 코드는?

A) `'Hello, ${"JS"}!'` B) ``Hello, ${"JS"}!`` C) `"Hello, ${"JS"}!"`

→ B

---
**8.** `"abc".length` 값은?

→ 3 (문자의 수)

---
**9.** `"Hello".toLowerCase()` 결과는?

→ hello (소문자 변경)

---
**10.** `"  hi  ".trim()` 결과는?

→ hi (공백 제거)

---
**11.** `"a,b,c".split(",")` 결과는?

→ ‘a’,’b’,’c’ (”,”로 구분)

---
**12.** `"abc".includes("b")` 는 `true`?

→ true (”b” 검색)

---
**13.** `"cat".replace("c","b")` 결과는?

→ bat (”c” → “b”)

---
**14.** 아래 출력결과는?

```jsx
console.log(2 == "2", 2 === "2");

// 정답
> true false

//'==' -> 알아서 타입을 변환하여 비교
//'===' -> 타입과 값 둘 다 비교
```

---
**15.** 삼항연산자 결과는?

```jsx
const n = 5;
const r = n % 2 === 0 ? "even" : "odd";

// 정답
> odd
```

---
**16.** switch 기본형에서 일치 비교에 쓰이는 것은?

A) ==  B) ===  C) 둘 다

→ B

---
**17.** && 단축 평가 결과:

```jsx
const ok = true && "DONE";

// 정답
> DONE
```

---
**18.** 속성 접근 결과?

```jsx
const user = { name: "Ann", age: 17 };
console.log(user["name"]);

// 정답
> Ann
```

---
**19.** 키를 추가한 다음 코드의 결과는?

```jsx
const k = "score";
const obj = {};
obj[k] = 100;
console.log(obj.score);

// 정답
> 100
```

---
**20.** 다음의 출력결과는?

```jsx
const a = { n: 1 };
const b = { n: 1 };
console.log(a === b);

// 정답
> true
```

---
**21.** const arr = [1,2,3]; arr.push(4); 이후 arr는?

→ index : 4 / value : (5)

---
**22.** pop()이 반환하는 것은?

→ 마지막 index를 꺼낸다.

---
**23.** slice(1,3)의 의미와 arr에 적용한 결과는?

→ index 1~2까지의(3직전)요소를 반환

---
**24.** splice(1,2)의 의미와 arr에 적용한 결과는?

→ index 1부터 2개의 요소를 반환하고 원본에서 삭제

---
**25.** map 결과?

```jsx
[1,2,3].map(x => x * 2)

// 정답
> 2,4,6
```

---
**26.** filter 결과?

```jsx
[1,2,3,4].filter(x => x % 2 === 0)

// 정답
> 2,4
```

---
**27.** includes 사용한 결과는?

```jsx
[1,2,3].includes(2)

// 정답
> true
```

---
**28.** reduce 결과는?

```jsx
[1,2,3].reduce((acc, cur) => acc + cur, 0)

// 정답
> 6
```

---
**29.** for (let i=0; i<3; i++) console.log(i); 출력?

→ 0 | 1 | 2

---
**30.** for...of는 어떤 것을 순회할때 효과적인가?

→ 배열의 인덱스나 객체의 키값

---
**31.** for...in은 주로 무엇을 순회할때 효과적인가?

→ 반복되는 속성

---
**32.** 다음 코드의 마지막 sum의 결과값은?

```jsx
let i=1, sum=0;
while(i<=3){ sum+=i; i++; }

// 정답
> 6
```

---
**33.** for...of 출력 결과는?

```jsx
for (const ch of "Hi") console.log(ch);

// 정답
> H
> i
```

---
**34.** 빈칸에 들어갈 키워드는 무엇인가?

```jsx
const arr = [10, 20, 30];
for (const num ___ arr) {
  console.log(num);
} 

// 정답
-> of
```

---
**35.** 아래 colors 배열의 요소값을 순서대로 출력하는 반복문을작성하세요

```jsx
const colors = ["red", "green", "blue"];

// 정답
-> 
colors.forEach (function (value) {
    console.log(value);
});
```

---
**36.** 아래  str의 요소를 순회하여 출력하는 반복문을 작성하세요.

```jsx
const str = "JS";

// 정답
->
for(const s of str){
    console.log(s)
}
```

---
**37.**  배열 scores의 점수에 대한  총점과 평균을 구하여 출력하는 코드를 작성하세요.

```jsx
const scores = [90, 80, 70];

// 정답
->
const total = scores.reduce((acc,cur)=> acc + cur,0);
const avg = total / scores.length;
```

---
**38.** 배열 nums 의 요소값 출력을 2번째 인덱스의 값까지만 출력하는 코드를 작성하세요

```jsx
const nums = [1, 2, 3];

// 정답
->
nums.slice(0,1)
```

---
**39.** user 객체의 정보를 출력하는 반복문을 작성하세요.

```jsx
const user = { name: "Yumi", age: 20 }; 

// 정답
->
for (let values in user) {
    console.log(values,user[values])
};
```

---
**40.** arr 배열의 요소값을 forEach문을 이용하여 출력하세요.

```jsx
const arr = [1, 2, 3];

// 정답
->
arr.forEach(function (value) {
    console.log(value)
});
```

---
**41.** `Map` 이란?

→ 키와 값이 한쌍으로 이루어진 컬렉션

---
**42.** `Set` 이란?

→ 중복되지 않는 값들의 집합

---
**43.** 아래 `Map의 결과는?`

```jsx
const m = new Map();
const k = {};
m.set(k, 123);
console.log(m.get(k));

// 정답
> 123
```

---
**44.** `Map` 크기 확인 프로퍼티는?

→ map.size