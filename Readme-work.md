## 相关代码说明

1.依据字体描述字符串fontStyle创建字体：D2UI::CFontPool::getSingleton().GetFont(fontStyle, 100);  
2.依据文字和字体计算显示宽度：pRT->MeasureText(pszText, _tcslen(pszText), &sz);  
3.属性文档：https://github.com/SOUI2/soui/blob/master/doc/soui%E5%B1%9E%E6%80%A7%E5%88%97%E8%A1%A8.xml  
