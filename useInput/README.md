# @noobs/use-input

useInput은 입력값의 상태를 관리하고, 필요에 따라 입력값을 검증할 수 있는 함수를 제공합니다.

## Installation:

yarn

```
yarn add @noobs/use-input
```

npm

```
npm i @noobs/use-input
```

## Arguments:

| Argument     | Type     | Description                                                              | Required |
| ------------ | -------- | ------------------------------------------------------------------------ | -------- |
| initialValue | string   | 입력 필드에 설정된 기본값 또는 초기값입니다.                             | yes      |
| validator    | function | 사용자 입력을 검증하는데 사용되는 사용자 지정 함수를 지정할 수 있습니다. | yes      |

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
