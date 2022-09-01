# windows11-classic-context-menu
<h2>Bring back old context menu (rightclick menu) in Windows 11</h2>
<hr>

<h3>New Windows 11 context menu:</h3>

![default](https://user-images.githubusercontent.com/101452307/158204636-368b1878-7569-435a-b347-4b5a5be79a27.png)

<p>There is much less options than in Windows 10.</p>

<h3>How to bring back context menu from Windows 10?</h3>

<p>In regedit find <b><i>CLSID</i></b> folder.</p>

<p>Location: [HKEY_CURRENT_USER\Software\Classes\CLSID]</p>

<p>Create new key named <code>{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}</code>.</p>

![reg1](https://user-images.githubusercontent.com/101452307/158205878-ea6e676f-ca5a-4617-aef0-377804fd0fc6.png)

![reg2](https://user-images.githubusercontent.com/101452307/158206012-b774e6c9-41c0-4824-a95e-57faf1bb8c9e.png)

<p>Inside <code>{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}</code> key create another one.</p>

<p>This time name it <code>InprocServer32</code>.</p>

![reg3](https://user-images.githubusercontent.com/101452307/158206574-67164858-e379-466a-a64a-e9a2f7c804d8.png)

![reg4](https://user-images.githubusercontent.com/101452307/158206598-ee1b515d-876e-4e35-a216-59cb96cf9f04.png)

<p>In <code>InprocServer32</code> double click the <code>Default</code> key.</p>

<p>Leave the <b><i>Value data</i></b> blank and click <b>OK</b>.</p>

![reg5](https://user-images.githubusercontent.com/101452307/158207279-7191628c-a0a8-46f0-b8f8-db94b3323315.png)

<p>After that restart your system.</p>

<h3>Results</h3>

<p>Enjoy the classic context menu in Windows 11.</p>

![patched](https://user-images.githubusercontent.com/101452307/158208040-5e87e93b-4d2e-4623-b6fe-8629580c4190.png)

<p>All in One Windows 11 Tewaks release in October</p>

<hr>
<h4><code>win11_classic_context_menu.reg</code> file will do this all for you.</h4>

