### [WebMonkey](https://github.com/warren-bank/Android-WebMonkey)

Minor improvement to the [WebView GM library](https://github.com/wbayer/webview-gm) demo application.

#### Background

* the [WebView GM library](https://github.com/wbayer/webview-gm) enhances the native Android System [WebView](https://developer.chrome.com/multidevice/webview/overview) with support for Greasemonkey functions and the management of user scripts

#### Improvements

* an additional Javascript API interface to provide the following functions to user scripts:
  - `GM_toastLong(message)`
  - `GM_toastShort(message)`
  - `GM_startIntent(data, ...extras)`
    * shows an Activity chooser to start an implicit Intent
    * where:
      - `data` is a String URL
      - `extras` is a list of String name/value pairs
    * example:
      - `('http://example.com/video.mp4', 'referUrl', 'http://example.com/videos.html')`
  - `GM_exit()`
    * causes [WebMonkey](https://github.com/warren-bank/Android-WebMonkey) to close

#### Legal:

* copyright: [Warren Bank](https://github.com/warren-bank)
* license: [GPL-2.0](https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt)
