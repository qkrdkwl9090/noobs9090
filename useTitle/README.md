# @noobs/use-title

useTitle 훅은 React 애플리케이션에서 웹 페이지의 타이틀을 동적으로 업데이트하는 데 사용됩니다. 이 훅을 사용하여 문서의 <title> 태그를 효율적으로 관리할 수 있습니다.

## Installation:

yarn

```
yarn add @noobs/use-title
```

npm

```
npm i @noobs/use-title

```

## Arguments:

| Argument     | Type   | Description                           | Required |
| ------------ | ------ | ------------------------------------- | -------- |
| initialTitle | string | 웹 페이지에 설정될 초기 타이틀입니다. | yes      |

## Usage:

```js
const TitleComponent = () => {
  const setTitle = useTitle("기본 타이틀"); // 초기 타이틀 설정

  return (
    <div>
      <button onClick={() => setTitle("새로운 타이틀")}>타이틀 변경</button>
    </div>
  );
};
```
