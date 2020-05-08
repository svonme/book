# mkdir

支持递归创建文件夹


```
const fs = require("fs");  
const path = require("path");

function mkdir(dirname) {
  // 判断文件夹是否存在
  if (fs.existsSync(dirname)) {
    return true;
  } else {
    // 递归执行创建任务
    if (mkdir(path.posix.dirname(dirname))) {
      // 创建文件夹
      fs.mkdirSync(dirname);
      return true;
    }
  }
}
```