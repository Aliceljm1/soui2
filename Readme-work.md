## 相关代码说明

1.依据字体描述字符串fontStyle创建字体：D2UI::CFontPool::getSingleton().GetFont(fontStyle, 100);  
2.依据文字和字体计算显示宽度：pRT->MeasureText(pszText, _tcslen(pszText), &sz);  
3.属性文档：https://github.com/SOUI2/soui/blob/master/doc/soui%E5%B1%9E%E6%80%A7%E5%88%97%E8%A1%A8.xml  

## 布局文件相关 
4.布局文件皮肤:xml\page_layout.xml 
5.主窗口布局 ：\demo\uires\xml\dlg_main.xml
6.初始化主窗口CMainDlg::OnInitDialog

## 类和控件说明
静态文本控件：SStatic, <text>	

绘制SkiaPath路径的自定义控件类：SPathView

渲染工厂类：SRenderFactory_Skia
可以创建各种渲染对象：CreateRenderTarget，CreateBitmap，CreatePath，CreateFont

渲染类：SRenderTarget_Skia
渲染方法：DrawBitmap，DrawPath，DrawText

## 其他核心方法
查找控件方法
	SWindow* SWindow::FindChildByName( LPCWSTR pszName , int nDeep)
创建子控件
	BOOL SWindow::CreateChildren(pugi::xml_node xmlNode)

