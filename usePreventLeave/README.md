# @noobs/use-prevent-leave

usePreventLeave 훅은 사용자가 실수로 웹 페이지를 벗어나는 것을 방지하는 데 사용됩니다. 이 훅은 beforeunload 이벤트를 활용하여 페이지를 벗어나기 전 사용자에게 경고 메시지를 표시할 수 있게 해줍니다.

## Installation:

yarn

```
yarn add @noobs/use-prevent-leave
```

npm

```
npm i @noobs/use-prevent-leave
```

## Usage:

```js
const InputComponent = () => {
  const maxLen = (value) => value.length <= 10;
  const name = useInput("initialValue", maxLen);

  return (
    <div>
      <input placeholder="Name" {...name} />
    </div>
  );
};
```
