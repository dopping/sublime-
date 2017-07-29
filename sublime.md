#关于sublime的配置信息

### sublime快捷键使用
- Ctrl+alt+f ==>格式化js代码
- Alt+shift+a==>局部代码格式化
- Alt+a ==> 侧边栏关闭和开启
- Alt+q ==> 页面在浏览器中打开

### sublime插件篇
- AdvancedNewFile ==> ctrl+alt+n ==> 建文件夹以及文件夹下面的文件 一步到位 不需要在侧边栏右键一个一个建立
- DocBlockr ==> 代码块注释 /*：回车注释一块代码，/**：回车在自动查找函数中的形参等等
- Jquery ==> jquery快捷使用方式 有提示，例如输入ajax会直接打出一下代码：
```
$.ajax({
            url: '/path/to/file',
            type: 'default GET (Other values: POST)',
            dataType: 'default: Intelligent Guess (Other values: xml, json, script, or html)',
            data: {param1: 'value1'},
        })
        .done(function() {
            console.log("success");
        })
        .fail(function() {
            console.log("error");
        })
        .always(function() {
            console.log("complete");
        });
```

### sublime主题篇
`开发主题1`
```
{
	"color_inactive_tabs": true,
	"color_scheme": "Packages/User/SublimeLinter/Afterglow-monokai (SL).tmTheme",
	"folder_no_icon": false,
	"font_size": 15,
	"ignored_packages":
	[
		"Vintage"
	],
	"sidebar_no_icon": false,
	"sidebar_row_padding_medium": true,
	"sidebar_size_14": true,
	"status_bar_brighter": true,
	"tabs_label_not_italic": true,
	"tabs_medium": true,
	"tabs_small": true,
	"theme": "Afterglow-magenta.sublime-theme",
	"word_wrap": true
}
```
---
`开发主题2`
```
{
	"color_inactive_tabs": true,
	"color_scheme": "Packages/User/SublimeLinter/base16-ocean.dark (SL).tmTheme",
	"enable_tab_scrolling": false,
	"folder_no_icon": false,
	"font_size": 16,
	"ignored_packages":
	[
		"Vintage"
	],
	"spacegray_fileicons": true,
	"spacegray_sidebar_font_xlarge": true,
	"spacegray_sidebar_tree_xlarge": true,
	"spacegray_tabs_auto_width": true,
	"spacegray_tabs_font_large": true,
	"spacegray_tabs_xlarge": true,
	"theme": "Spacegray.sublime-theme",
	"word_wrap": true
}
```
---
###按键绑定
```
[

    // chrome
    {
        "keys": ["alt+q"],
        "command": "side_bar_files_open_with",
        "args": {
            "paths": [],
            "application": "C:/Program Files (x86)/Google/Chrome/Application/chrome.exe",
            "extensions": ".*"
        }
    },

    // firefox
    {
        "keys": ["f3"],
        "command": "side_bar_files_open_with",
        "args": {
            "paths": [],
            "application": "D:/Program Files (x86)/Mozilla Firefox/firefox.exe",
            "extensions": ".*"
        }
    },

    // ie
    {
        "keys": ["f4"],
        "command": "side_bar_files_open_with",
        "args": {
            "paths": [],
            "application": "C:/Program Files/Internet Explorer/iexplore.exe",
            "extensions": ".*"
        }
    },
    {
        "keys": ["alt+a"],
        "command": "toggle_side_bar"
    },
    //代码格式化快捷键
    {
        "keys": ["alt+shift+a"],
        "command": "reindent"
    },
    //在浏览器中打开markdown编辑的文件
    {
        "keys": ["f5"],
        "command": "markdown_preview",
        "args": {
            "target": "browser",
            "parser": "markdown"
        }
    },

]
```