# @noobs/use-before-leave

useBeforeLeave 훅은 사용자의 마우스 포인터가 브라우저 창을 벗어나는 순간을 감지하고, 이에 대응하는 사용자 정의 행동을 수행하게 해주는 훅입니다. 이 훅은 mouseleave 이벤트를 활용하여 마우스 포인터가 브라우저 창 상단을 벗어날 때 호출됩니다.

## Installation:

yarn

```
yarn add @noobs/use-before-leave
```

npm

```
npm i @noobs/use-before-leave
```

## Arguments:

| Argument | Type     | Description                                         | Required |
| -------- | -------- | --------------------------------------------------- | -------- |
| onBefore | function | 마우스가 브라우저 창을 벗어날 때 실행될 함수입니다. | yes      |

## Usage:

```js
const BeforeLeaveComponent = () => {
  const handleBeforeLeave = () => console.log("Don't leave!");
  useBeforeLeave(handleBeforeLeave);

  return (
    <div>
      <h1>Hello!</h1>
    </div>
  );
};
```
