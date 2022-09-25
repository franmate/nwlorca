# Lorca


<div>

<br/>
<p>
	A very small library to build modern HTML5 desktop apps in Go. It uses Chrome
	browser as a UI layer. Unlike Electron it doesn't bundle Chrome into the app
	package, but rather reuses the one that is already installed. Lorca
	establishes a connection to the browser window and allows calling Go code
	from the UI and manipulating UI from Go in a seamless manner.
</p>
<br/>
</div>


## Features

* Pure Go library (no cgo) with a very simple API
* Small application size (normally 5-10MB)
* Best of both worlds - the whole power of HTML/CSS to make your UI look
	good, combined with Go performance and ease of development
* Expose Go functions/methods and call them from JavaScript
* Call arbitrary JavaScript code from Go
* Asynchronous flow between UI and main app in both languages (async/await and Goroutines)
* Supports loading web UI from the local web server or via data URL
* Supports testing your app with the UI in the headless mode
* Supports multiple app windows
* Supports packaging and branding (e.g. custom app icons). Packaging for all
	three OS can be done on a single machine using GOOS and GOARCH variables.

Also, limitations by design:

* Requires Chrome/Chromium >= 70 to be installed.
* No control over the Chrome window yet (e.g. you can't remove border, make it
	transparent, control position or size).
* No window menu (tray menus and native OS dialogs are still possible via
	3rd-party libraries)


Code is distributed under MIT license, feel free to use it in your proprietary
projects as well.

