# @noobs/use-confirm

useConfirm 훅은 사용자의 확인을 요구하는 상황에서 사용됩니다. 이 훅은 confirm 대화 상자를 통해 사용자에게 메시지를 보여주고, 사용자의 응답에 따라 다른 행동을 취할 수 있도록 합니다.

## Installation:

yarn

```
yarn add @noobs/use-confirm
```

npm

```
npm i @noobs/use-confirm
```

## Arguments:

| Argument  | Type     | Description                                      | Required |
| --------- | -------- | ------------------------------------------------ | -------- |
| message   | string   | confirm 대화 상자에 표시될 메시지입니다.         | no       |
| onConfirm | function | 사용자가 '확인'을 클릭했을 때 호출될 함수입니다. | yes      |
| onCancel  | function | 사용자가 '취소'를 클릭했을 때 호출될 함수입니다. | yes      |

## Usage:

```js
const ConfirmComponent = () => {
  const deleteWorld = () => console.log("Deleting the world...");
  const abort = () => console.log("Aborted");
  const confirmDelete = useConfirm("Are you sure?", deleteWorld, abort);

  return (
    <button onClick={confirmDelete}>Delete the world</button>
  );
};
};
```
