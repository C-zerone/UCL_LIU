# UCL_LIU
利用python+pyhook開發的仿蝦米，肥米輸入法<br>
<br>
<center>
  <img src="http://3wa.tw/uploads/upload/ucl_2.png">
</center>
<br>
作者：羽山秋人 (<a target="_blank" href="http://3wa.tw">http://3wa.tw</a>)<br>
<br>
版本：V 0.1<br>
<br>
開發動機：<br>
　　吃飽閒閒覺得人生就是該自己寫一套輸入法，然後就開始寫了。<br>
字碼表；<br>
　　由於字碼表的版權問題，我就不放 liu.json 了，liu.json 的格式同PIME的架構。<br>
   要好的字碼表的話，請買正版，將 tab->cin->json <br>
   雖然很麻煩，但沒人想因為實作一套輸入法就被告翻。<br>
<br>
開發工具：<br>
  <ul>
    <li>Python 27 (32BIT)</li>
    <li>pyhook</li>
    <li>pygtk</li>
    <li>pywin32</li>
    <li>pyinstaller 可搭配build.bat製作dist/uclliu.exe檔</li>
    <li>(Third party) portalocker.py 防重複執行，會Lock C:\tmp\</li>
    <li>(Third party) SendKeysCtypes.py 可以送出Unicode的SendKeys</li>
    <li>字碼表參考PIME裡的liu.json</li>
</ul>
<br>
編譯：<br>
　　pip install pyinstaller<br>
    參考 build.bat 製作單一 exe 方法<br>
<br>  
ToDo：<br>
<ul>
  <li>(Done)<s>1、(嚴重)「送出字元」的方法，試了很多send key一直無法解決 send unicode的問題，暫時使用「剪貼簿」的Ctrl+V來實作貼上文字的功能</s></li>
  <li>2、「英文全形」輸入時，有些組合鍵如 Alt+tab還尚未決定</li>
  <li>(Done)<s>3、py2exe包成一支exe</s>改用pyinstaller代替</li>
  <li>4、尚有些按鍵會讓「英/肥」切來切去，暫未處理</li>
  <li>(Done)<s>5、離開程式的按鈕</s></li>
  <li>(Done)<s>6、支援V鍵選第二個字</s></li>
  <li>(Done)<s>7、「」【】這種框框應該也要支援</s></li>
  <li>(Done)<s>8、sendkey時，判斷window id，如果該id是putty、pcman，改成shift+ins作文字貼上</s></li>
  <li>(Done)<s>9、「英/半」時，加上調整opacity值，讓肥米變透明(Opacity 0.2)</s></li>
  <li>(Done)<s>10、增加提示沒有liu.json時的錯誤警告</s></li>
  <li>11、輸出字後，可以[提示簡根字]，以便提升打字速度</li>
  <li>12、同音字查詢</li>
  <li>13、寫一篇如何把tab->cin->json的教學</li>
  <li>14、支援把tab跟UCLLIU放一起就可以自動使用、轉檔的功能</li>
  <li>15、缺碼查詢，如lom[、lom]</li>
  <li>16、在「英/全」的模式時，無法按 Shift 切換回「肥/全」</li>
  <li>17、在「肥/全」的「冒號」應該是要出全形字，「分號」要出全型字
  <li>18、支援Linux、Mac的研究(下一次吃飽閒閒再說)</li>    
</ul>
<br>
版權：<br>
　MIT-License
