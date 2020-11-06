# form-render-excel

![](https://img.shields.io/npm/v/form-render-excel.svg)
![](https://img.shields.io/npm/dt/form-render-excel.svg)

## 安装

```bash
npm i form-render-excel --save
```

## 使用

```jsx
import React, { useState } from 'react';
import 'antd/dist/antd.css';
import FR from 'form-render/lib/antd';
import HOC from 'form-render-excel';
import schema from './schema.json';

// 把原来的 FormRender 包一下
const NFR = HOC(FR);

export default () => {
  const [formData, setFormData] = useState({});

  // 当成正常的 FormRender 来使用
  return <NFR schema={schema} formData={formData} onChange={setFormData} />;
};
```

## 功能

支持复杂的数组多层套对象的导入导出，可以 clone 下代码，跑起来试玩一下~

### 导出功能

![](https://img.alicdn.com/tfs/TB1jr5r1bY1gK0jSZTEXXXDQVXa-2138-1162.png)

### 导入功能

![](https://img.alicdn.com/tfs/TB1nGqB1kL0gK0jSZFAXXcA9pXa-2052-1474.png)
