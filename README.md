B4X實驗: 不可錯過的B4X BANano網頁包裝工具.直覺式建立CRUD網站篇-Bootstrap CSS..Not perfect!!MayBe you can modify
參考資料:
https://www.b4x.com/android/forum/threads/sithasodaisy-tailwindcss-webapps-using-b4x.143950/
SithasoDaisy: TailwindCss WebApps using B4x


0.BANano???
BANano 為您提供了一套工具來圍繞任何框架（MiniCSS、Skeleton、Spectre、Bootstrap 等）編寫您自己的包裝器，
然後可以輕鬆地使用它們來快速構建 web 應用程序/網站。

0.請問登入api傳賬號、密碼json明碼會有問題嗎?  (資安議題)
https://ithelp.ithome.com.tw/questions/10211642?sc=nl.daily


1.展示用B4X BANano建立網站-使用Bootstrap CSS框架.美化網站
https://b234.top/

2.簡單直覺式 程式碼!!!




使用BANanoElement撰寫

	Dim body As BANanoElement
	body.Initialize("#body")
   
	Dim form As BANanoElement
	form.Initialize("<form>") 'make a new form tag
   
	Dim input As BANanoElement
	input.Initialize("<input>") 'make a new input tag
	input.SetAttr("id", "mycheck")
	input.SetAttr("type", "checkbox")
	input.On("mouseover", Me, "hoverit")
	input.On("click", Me, "clickit")
	form.Append(input)
	body.Append(form)
   
	Dim btnTD As BANanoElement
	btnTD.Initialize("<button>") ' make a new button tag
	btnTD.SetText("Toggle Text Direction")
	btnTD.On("click", Me, "Toggledir")
	body.Append(btnTD)
   
	Dim p As BANanoElement
	p.Initialize("<p>") ' make a new p tag
	p.SetAttr("id", "note")
	p.Settext("Hover over the checkbox to simulate a click")
	body.Append(p)

對於直覺來說.不夠?但它提共了一個基礎!!
---------------------------------------------------
經過我改良的.(參考 SithasoDaisy: TailwindCss WebApps using B4x )


我自己練習寫了一套類似的
不完美!!MayBe你可以修改


0.當我愈熟悉.愈加肯定!!BaNano 是一個非常棒的網頁包裝程式

提共了很多HTML/CSS/JavaScript相關的應用
靈活..但又不會成學習負擔!!!!

當然你會說用其他語言包裝html元素成為物件.前後端的語言工具比如jq/javascript/vue/php/....
(vue包裝元件.這我玩過)
>>我只花了一個月多.實地手工打造.一些基礎的html元件 textbox.....
>>包裝一個DataTable物件...(網上有名的DataTable/jqGrid.)
>>並且 優化 CRUD 範例.....
>>事實證明!!BaNano是最容易使用並理解的網頁包裝程式庫


最後.因為被我包裝過.看似難!!其實.看程式碼.要用物件的語意去理解!!學習將很容易~~~~
我這非學霸的腦袋.都能做出來了.相信!!你.行的


'版別:20230215
'作者:eric19740521@gmail.com
'https://www.youtube.com/ 上面搜尋B4X.可找到相關影片
'捐獻:努力的成果.得來不易!!認同!可隨意捐款!! 台灣 700郵局 帳號02913630064001


