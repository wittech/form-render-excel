# form-render-excel

## 安装

```bash
npm i form-render-excel --save
```

## 功能

### 导出功能

![](https://img.alicdn.com/tfs/TB1jr5r1bY1gK0jSZTEXXXDQVXa-2138-1162.png)

### 导入功能

![](https://img.alicdn.com/tfs/TB1nGqB1kL0gK0jSZFAXXcA9pXa-2052-1474.png)

## 使用
```jsx
import React, { useState } from 'react';
import 'antd/dist/antd.css';
import FR from "form-render/lib/antd";
import HOC from 'form-render-excel';
import schema from "./schema.json";

// 把原来的 FormRender 包一下
const NFR = HOC(FR);

export default () => {
  const [formData, setFormData ] = useState({});

  return <NFR schema={schema} formData={formData} onChange={setFormData} />
}
```