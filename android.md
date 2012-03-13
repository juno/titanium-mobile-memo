Titanium Mobile Memo (Android)
====


SDカードへのインストールを許可する`tiapp.xml`
----

     <android xmlns:android="http://schemas.android.com/apk/res/android">
-        <manifest>
+        <tool-api-level>8</tool-api-level>
+        <manifest android:versionCode="1" android:versionName="1.0" android:installLocation="auto">
             <supports-screens android:anyDensity="false"
                 android:largeScreens="true" android:normalScreens="true" android:smallScreens="false"/>
+            <uses-sdk android:minSdkVersion="8" android:targetSdkVersion="8" />
         </manifest>
     </android>


Androidでは`TableView`の`index`がずれる
----

* [(Android) Tableview: updateRow with headers » Community Questions &amp; Answers » Appcelerator Developer Center](http://developer.appcelerator.com/question/10131/android-tableview-updaterow-with-headers)


Androidではヘッダを持つTableViewのupdateRowでOut of boundになる
----

work in progress.



