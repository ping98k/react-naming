# react-conventions

File naming conventions in react



## camelCase

variable that can process in app

```TSX
let itemList = [];
const myFunction = () => {};
```


## PascalCase

`class`, `type`, `enum`, `interface`, `const`, `component`

```TSX
enum Shape {Circle,Square}
type MyButtonProps = { shape?: Shape };
const MyButton = (props: MyButtonProps) => <button />;
const myButton = <MyButton shape={Shape.Circle} />;
```


## kebab-case

### file and folder name which not executable

```
/my-images/default-profile.png
/my-images/index.tsx
```

```TSX
export const my_images =  {
  default_profile: "./default-profile.png",
};
```

### file export data

```
/my-components/MyButton/MyButton.tsx
/my-components/MyButton/MyButton.hook.tsx
/my-components/MyButton/MyButton.pure.tsx
/my-components/MyButton/MyButton.style.tsx

/constants/colors.ts
/constants/storage_keys.ts
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

constant that can process in app

```TSX
const app_configs = {
    max_item: 10,
    max_timeout: 6000,
};

const itemList = [];
if (itemList.length <= app_configs.max_item) {
    itemList.push("123");
}
```


## UPPER_SNAKE_CASE

constant that communicate with another program

```TSX
export const configs = {
  WEB_BASE_URL: "https://www.my-web.com/",
  API_BASE_URL: "https://www.my-api.com/",
};

export const storage_keys = {
  NAVIGATION_STATE: "NAVIGATION_STATE",
  USER_CACHE: "USER_CACHE",
};

export const collection_names = {
  USER_PROFILE: "userProfile",
  COURSES: "courses",
};
```