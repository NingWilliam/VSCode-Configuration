VSCode 云同步扩展设置Setting Sync插件：

```
https://www.jb51.net/article/186057.htm
```



Unable to read syncLocalSettings.json. Make sure its Valid JSON. 报错解决方法：

```
https://www.cnblogs.com/zjhblogs/p/13214234.html
```

Git ID：33a7132ee48cc64574a8c60de815823fc3e3eaca

Gist ID：7cf64821776d75aa4bacd2fa97246680



setting.json文件配置：

```
{

 // 启用/禁用导航路径。

 "breadcrumbs.enabled": true,

 // 控制缩进空格数。

 "editor.tabSize": 2,

 // 控制字体大小。

 "editor.fontSize": 18,

 // 控制字体行高。

 "editor.lineHeight": 26,

 // 控制编辑器在空白字符上显示符号的方式。

 "editor.renderWhitespace": "boundary",

 // 控制光标的动画样式。

 "editor.cursorBlinking": "smooth",

 // 渲染每行的实际字符，而不是色块。

 "editor.minimap.renderCharacters": false,

 // 控制字体系列。

 "editor.fontFamily": "'Fira Code', 'Droid Sans Mono', 'Courier New', monospace, 'Droid Sans Fallback'",

 // 启用/禁用字体连字。

 "editor.fontLigatures": true,

 // 按住 Ctrl 键并滚动鼠标滚轮时对编辑器字体大小进行缩放。

 "editor.mouseWheelZoom": false,



 //autoFixedOnSave 设置已废弃，采用如下新的设置

 "editor.codeActionsOnSave": {

  "source.fixAll.eslint": true

 },

 "eslint.format.enable": true,

 //autoFix默认开启，只需输入字符串数组即可

 "eslint.validate": **[**"javascript", "vue", "html"**]**,

 "vetur.format.defaultFormatter.js": "vscode-typescript",

 // 控制是否在打开文件时，基于文件内容自动检测

 "editor.detectIndentation": false,

 // 控制在资源管理器内拖放移动文件或文件夹时是否进行确认。

 "explorer.confirmDragAndDrop": false,

 // 启用后，保存文件时在文件末尾插入一个最终新行。

 "files.insertFinalNewline": true,

 // 启用时，提交将自动从当前Git存储库的默认远程获取。

 "git.autofetch": true,

 // Git 可执行文件的路径和文件名。

 "git.path": "F:\\Program Files\\Git\\cmd\\git.exe",

 // 配置glob模式以在全文本搜索和快速打开中排除文件和文件夹。

 "search.exclude": {

  "**/node_modules": true,

  "**/dist": true

 },

 // 区域的默认格式化程序-HTML格式化程序。

 "vetur.format.defaultFormatter.html": "js-beautify-html",

 // 区域的默认格式化程序。

 "vetur.format.defaultFormatter.ts": "vscode-typescript",

 // 设置在报告 JavaScript 和 TypeScript 的错误时使用的区域设置。

 "typescript.locale": "en",

 // 调整窗口标题栏的外观。

 "window.titleBarStyle": "custom",

 // 控制工作台中活动栏的可见性。

 "workbench.activityBar.visible": true,

 // 指定用在工作台中的颜色主题。

 "workbench.colorTheme": "Flat UI (+GUI)",

 // 在保存时运行的代码操作类型。

 "editor.codeActionsOnSave": {

  "source.fixAll.eslint": true

 },

 // 指定工作台中使用的文件图标主题。

 "workbench.iconTheme": "Monokai Pro (Filter Octagon) Icons",



 // 指定每行代码的最佳长度， 如果超出长度则换行。

 "prettier.printWidth": 120,



 // 如果为 true，将使用单引号而不是双引号。

 "prettier.singleQuote": true,

 // 是否在每行末尾添加分号。

 "prettier.semi": false,

 // 在保存时格式化文件。

 "editor.formatOnSave": true,
 
 // 强制单引号
 
 "prettier.singleQuote": true,
 
 // 控制尾随逗号的打印
 
 "prettier.trailingComma": "all",
 
 // 开启 exlint 支持
 
 "prettier.eslintIntegration": true,
 
 // 使用插件格式化 html
 
 “vutur.format.defaultFormatter.html”: "js-beautify-html",
 
 // 格式化插件的配置
 
 "vetur.format.defaultFormartterOptions": {
 
 "js-beautify-html": {
 
           // 属性强制折行对齐
           
           "warp_attributes": "force-aligned"
           
       }
       
 },
 // 启用/禁用 JavaScript 格式化程序。

 "javascript.format.enable": false,

 "[vue]": {

  "editor.defaultFormatter": "esbenp.prettier-vscode",

  "editor.formatOnType": false,

  "editor.formatOnSave": false

 },

 "emmet.includeLanguages": {},

 "editor.wordWrap": "on",

 "editor.wordWrapColumn": 240,

 "workbench.colorCustomizations": {

  "editor.selectionBackground": "#00a2ff" // 编辑器所选内容的颜色

 },

 "files.autoSave": "onFocusChange",

 "eslint.autoFixOnSave": true,

 "sync.gist": "7cf64821776d75aa4bacd2fa97246680",

 "sync.autoUpload": true

}

https://github.com/NingWilliam/VSCode-Configuration/blob/master/image-20200717/image-20200717145757885.png

