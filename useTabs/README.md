# @noobs/use-tabs

useTabs 훅은 탭 인터페이스를 구현하는 데 사용되며, 현재 선택된 탭의 상태를 관리하고 변경할 수 있는 기능을 제공합니다.

## Installation:

yarn

```
yarn add @noobs/use-tabs
```

npm

```
npm i @noobs/use-tabs

```

## Arguments:

| Argument   | Type   | Description                      | Required |
| ---------- | ------ | -------------------------------- | -------- |
| initialTab | number | 초기에 선택될 탭의 인덱스입니다. | yes      |
| allTabs    | array  | 탭 데이터를 포함하는 배열입니다. | yes      |

## Usage:

```js
const tabsData = [
  { title: "Tab 1", content: "This is Tab 1" },
  { title: "Tab 2", content: "This is Tab 2" },
];

const TabsComponent = () => {
  const { currentItem, changeItem } = useTabs(0, tabsData);
  return (
    <div>
      {tabsData.map((tab, index) => (
        <button key={index} onClick={() => changeItem(index)}>
          {tab.title}
        </button>
      ))}
      <div>{currentItem.content}</div>
    </div>
  );
};
```
