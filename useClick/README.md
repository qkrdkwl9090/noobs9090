# @noobs/use-click

useClick 훅은 React 애플리케이션에서 클릭 이벤트 리스너를 쉽게 관리할 수 있게 해주는 훅입니다. 이 훅을 사용하여 특정 DOM 요소에 클릭 이벤트 핸들러를 추가하고 제거할 수 있습니다.

## Installation:

yarn

```
yarn add @noobs/use-click
```

npm

```
npm i @noobs/use-click

```

## Arguments:

| Argument | Type     | Description                                 | Required |
| -------- | -------- | ------------------------------------------- | -------- |
| onClick  | function | 클릭 이벤트 발생 시 호출될 콜백 함수입니다. | yes      |

## Usage:

```js
const ClickComponent = () => {
  const sayHello = () => console.log("Hello!");
  const title = useClick(sayHello);

  return <h1 ref={title}>Hello!</h1>;
};
```
