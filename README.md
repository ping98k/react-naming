# react-conventions

File naming conventions in react

## UPPER_CASE_SNAKE_CASE

constant that communicate with another program

```TSX
export const configs = {
  WEB_BASE_URL: "https://www.my-web.com/",
  API_BASE_URL: "https://www.my-api.com/",
};

export const storageKeys = {
  NAVIGATION_STATE: "NAVIGATION_STATE",
  USER_CACHE: "USER_CACHE",
};

export const collectionNames = {
  USER_PROFILE: "userProfile",
  COURSES: "courses",
};
```

## PascalCase

`class`, `type`, `enum`, `interface`

```TSX
type MyButtonProps = { title: string };
const MyButton = (props: MyButtonProps) => <button>{props.title}</button>;
```

## kebab-case
file and folder name which not executable
```
/my-images/default-profile.png
/my-images/index.tsx
```
```TSX
export const myImages =  {
  default_profile: "./default-profile.png",
};
```

## snake_case
constant that communicate with user

```TSX
export const colors = {
  alpha_text: "#A3B9C9",
  alpha_background: "#776D5A",
  beta_text: "#987D7C",
  beta_background: " #ABDAE1",
};

export const en = {
  file_naming_conventions_in_react: "File naming conventions in react",
};

```

## camelCase
variable that can process in app

```TSX
const appConfigs = {
  maxItem: 10,
  maxTimeout: 6000,
};

const itemList = [];
if (itemList.length <= appConfigs.maxItem) {
  itemList.push("123");
}

```