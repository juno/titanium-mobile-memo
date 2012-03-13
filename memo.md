Titanium Mobile Memo
====


`Ti.UI.TableView`のフォントサイズを指定することはできない
----

かわりに`Ti.UI.Label`を`TableViewRow`に`add`して使う。

    row = Ti.UI.createTableViewRow
    label = Ti.UI.createLabel
      color: '#000'
      font: { fontSize: 16 }
      left: 10
      text: 'Hello'
    row.add(label)

* [titanium_mobile/demos/KitchenSink/Resources/examples/table_view_layout_2.js at master · appcelerator/titanium_mobile](https://github.com/appcelerator/titanium_mobile/blob/master/demos/KitchenSink/Resources/examples/table_view_layout_2.js)


`currentTab`と`currentWindow`
----

CurrentTab specifies the tab owning the window owning the context. That is, it's akin to currentWindow. The code sample in question is in app.js, which is not owned by any window, thus, no currentWindow, no currentTab.

* [[#TIMOB-2797] Ti.UI.currentTab is null - Appcelerator JIRA](https://jira.appcelerator.org/browse/TIMOB-2797)


Windowに完了ボタンを表示する
----

    if Ti.Platform.name is 'iPhone OS'
      doneButton = Ti.UI.createButton(systemButton: Ti.UI.iPhone.SystemButton.DONE)
      self.setRightNavButton(doneButton)


"Adding an event listener to a proxy that isn't already in the context"
----

* [[ERROR] Adding an event listener to a proxy that isn&apos;t already in the context » Community Questions &amp; Answers » Appcelerator Developer Center](http://developer.appcelerator.com/question/131453/error-adding-an-event-listener-to-a-proxy-that-isnt-already-in-the-context)
* [[#TIMOB-7347] iOS: TextArea - In KS, Scroll Views Text Area test is printing out error messages to the console - Appcelerator JIRA](https://jira.appcelerator.org/browse/TIMOB-7347)


フリップトランジション
----

    params.transition = Titanium.UI.iPhone.AnimationStyle.FLIP_FROM_RIGHT unless Ti.App.isAndroid


モーダルウィンドウのネストはできない
----

* [Modal Window open another Modal Window, how? » Community Questions &amp; Answers » Appcelerator Developer Center](http://developer.appcelerator.com/question/129792/modal-window-open-another-modal-window-how)


OSの書式化機能
----

`String`オブジェクトに関数が定義されている。

    format (formatString, value)
    formatCurrency (value)
    formatDate (date, format)
    formatDecimal (value)
    formatTime (date)

表示例。

    [DEBUG] short date: 2/26/12
    [DEBUG] medium date: 2/26/12
    [DEBUG] long date: February 26, 2012
    [DEBUG] short time: 3:34 PM
    [DEBUG] medium time: 3:34:31 PM
    [DEBUG] long time: 3:34:31 PM GMT+09:00


Graph APIのProfileは直接取得できる
----

* [http://graph.facebook.com/userid/picture](http://developer.appcelerator.com/question/117746/facebook-user-pic-response)

* [Button in textfield - [error] style:Titanium.UI.iPhone.SystemButton.DISCLOSURE » Community Questions &amp; Answers » Appcelerator Developer Center](http://developer.appcelerator.com/question/118142/button-in-textfield---error-styletitaniumuiiphonesystembuttondisclosure)


Graph APIでvenueにlatitudeを設定できない
----

* Facebook Graph APIの既知の問題
