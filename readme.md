## 부록

##### setTimeout()

- setTimeout() 함수는 첫번째 인자로 실행할 코드를 담고 있는 함수를 받고, 두번째 인자로 지연 시간을 밀리초(ms) 단위로 받습니다.

```js
setTimeout(() => console.log('2초 후에 실행됨'), 2000);
const timeoutId = setTimeout(() => console.log('5초 후에 실행됨'), 5000);
clearTimeout(timeoutId);
```

##### setInterval()

- setInterval() 함수는 어떤 코드를 일정한 시간 간격을 두고 반복해서 실행하고 싶을 때 사용합니다

- clearInterval() 함수를 호출하면 코드가 주기적으로 실행되는 것을 중단

```js
setInterval(() => console.log(new Date()), 2000);

const intervalId = setInterval(() => console.log(new Date()), 2000);
```

`너무 많은 코드들이 표시된다... ㅠㅠ 그럴 땐 멈추는 함수는`

- clearInterval() 함수를 호출하면 코드가 주기적으로 실행되는 것을 중단

```js
clearInterval(intervalId);
```

##### canvas()

- canvas의 드로잉 컨텍스트를 정의하는 컨텍스트를 식별자이며 다음 아래의 값을 가질 수 있다.

```js
const canvas = document.getElementById('canvas');
const canvasContext = canvas.getContext('2d');
```
