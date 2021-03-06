# راهنمای رسمی

لطفا مطمئن شوید که شما با استفاده از اسناد نسخه الکترون را مطابقت میدهید . شماره نسخه باید بخشی از URL صفحه باشد. اگر اینطور نمی باشد، شما احتمالا از مستندات گروه توسعه که حاوی تغییرات API است و سازگار با نسخه ای الکترونی شما نیست استفاده میکنید. برای دیدن قدیمی تر نسخه های اسناد، شما می توانید [ مرور بر اساس برچسب ](https://github.com/electron/electron/tree/v1.4.0) در GitHub با باز کردن 'منوی شاخه ها / برچسب ها' کشویی و انتخاب برچسبی که مطابق نسخه شما است.

## سوالات متداول

سوالاتی وجود دارد که از اغلب آنها خواسته می شود. قبل از ایجاد یک مسئله آن را بررسی کنید:

* [سوالات متداول الکترون](faq.md)

## راهنماها و آموزشها

* [راه اندازی محیط توسعه](tutorial/development-environment.md) 
  * [راه اندازی macOS](tutorial/development-environment.md#setting-up-macos)
  * [راه اندازی ویندوز](tutorial/development-environment.md#setting-up-windows)
  * [راه اندازی لینوکس](tutorial/development-environment.md#setting-up-linux)
  * [انتخاب یک ویرایشگر](tutorial/development-environment.md#a-good-editor)
* [ایجاد اولین برنامه شما](tutorial/first-app.md) 
  * [نصب الکترون Electron](tutorial/first-app.md#installing-electron)
  * [توسعه الکترون به طور کلی](tutorial/first-app.md#electron-development-in-a-nutshell)
  * [app در حال اجرای خود را](tutorial/first-app.md#running-your-app)
* [Boilerplates و همچنین CLIs ](tutorial/boilerplates-and-clis.md) 
  * [Boilerplate در مقابل CLI](tutorial/boilerplates-and-clis.md#boilerplate-vs-cli)
  * [electron-forge](tutorial/boilerplates-and-clis.md#electron-forge)
  * [electron-builder](tutorial/boilerplates-and-clis.md#electron-builder)
  * [electron-react-boilerplate](tutorial/boilerplates-and-clis.md#electron-react-boilerplate)
  * [سایر ابزارها و Boilerplates](tutorial/boilerplates-and-clis.md#other-tools-and-boilerplates)
* [معماری برنامه](tutorial/application-architecture.md) 
  * [فرآیندهای اصلی و رندرینگ](tutorial/application-architecture.md#main-and-renderer-processes)
  * [استفاده از API های الکترونی](tutorial/application-architecture.md#using-electron-apis)
  * [استفاده از API های Node.js](tutorial/application-architecture.md#using-nodejs-apis)
  * [Using Native Node.js Modules](tutorial/using-native-node-modules.md)
* Adding Features to Your App 
  * [Notifications](tutorial/notifications.md)
  * [Recent Documents](tutorial/desktop-environment-integration.md#recent-documents)
  * [Application Progress](tutorial/progress-bar.md)
  * [Custom Dock Menu](tutorial/macos-dock.md)
  * [وظیفه سفارشی سازی ویندوز](tutorial/windows-taskbar.md)
  * [عملیات سفارشی لینوکس دسکتاپ](tutorial/linux-desktop-actions.md)
  * [میانبرهای صفحه کلید](tutorial/keyboard-shortcuts.md)
  * [ تشخیص آفلاین / آنلاین](tutorial/online-offline-events.md)
  * [نمایه فایل برای macOS BrowserWindows](tutorial/represented-file.md)
  * [Native File Drag & Drop](tutorial/native-file-drag-drop.md)
* [دسترسی](tutorial/accessibility.md) 
  * [اسپکترون](tutorial/accessibility.md#spectron)
  * [Devtron](tutorial/accessibility.md#devtron)
  * [فعال کردن قابلیت دسترسی](tutorial/accessibility.md#enabling-accessibility)
* [تست و اشکال زدایی](tutorial/application-debugging.md) 
  * [اشکال زدایی فرآیند اصلی ](tutorial/debugging-main-process.md)
  * [استفاده از Selenium و WebDriver](tutorial/using-selenium-and-webdriver.md)
  * [تست سیستم های CI (Travis، Jenkins)](tutorial/testing-on-headless-ci.md)
  * [افزونه DevTools](tutorial/devtools-extension.md)
  * [تست خودکار با یک درایور سفارشی](tutorial/automated-testing-with-a-custom-driver.md)
* پکها 
  * [Code Signing](tutorial/code-signing.md)
* [توضیع](tutorial/application-distribution.md) 
  * [پشتیبانی](tutorial/support.md)
  * [فروشگاه Mac App Store](tutorial/mac-app-store-submission-guide.md)
  * [فروشگاه ویندوز](tutorial/windows-store-guide.md)
  * [Snapcraft](tutorial/snapcraft.md)
* [Security](tutorial/security.md) 
  * [Reporting Security Issues](tutorial/security.md#reporting-security-issues)
  * [Chromium Security Issues and Upgrades](tutorial/security.md#chromium-security-issues-and-upgrades)
  * [Electron Security Warnings](tutorial/security.md#electron-security-warnings)
  * [Security Checklist](tutorial/security.md#checklist-security-recommendations)
* [Updates](tutorial/updates.md) 
  * [Deploying an Update Server](tutorial/updates.md#deploying-an-update-server)
  * [Implementing Updates in Your App](tutorial/updates.md#implementing-updates-in-your-app)
  * [Applying Updates](tutorial/updates.md#applying-updates)

## Detailed Tutorials

These individual tutorials expand on topics discussed in the guide above.

* [In Detail: Installing Electron](tutorial/installation.md) 
  * [Proxies](tutorial/installation.md#proxies)
  * [Custom Mirrors and Caches](tutorial/installation.md#custom-mirrors-and-caches)
  * [Troubleshooting](tutorial/installation.md#troubleshooting)
* [In Detail: Electron's Versioning Scheme](tutorial/electron-versioning.md) 
  * [semver](tutorial/electron-versioning.md#semver)
  * [Stabilization Branches](tutorial/electron-versioning.md#stabilization-branches)
  * [Beta Releases and Bug Fixes](tutorial/electron-versioning.md#beta-releases-and-bug-fixes)
* [In Detail: Packaging App Source Code with asar](tutorial/application-packaging.md) 
  * [Generating asar Archives](tutorial/application-packaging.md#generating-asar-archives)
  * [Using asar Archives](tutorial/application-packaging.md#using-asar-archives)
  * [محدودیت ها](tutorial/application-packaging.md#limitations-of-the-node-api)
  * [Adding Unpacked Files to asar Archives](tutorial/application-packaging.md#adding-unpacked-files-to-asar-archives)
* [In Detail: Using Pepper Flash Plugin](tutorial/using-pepper-flash-plugin.md)
* [In Detail: Using Widevine CDM Plugin](tutorial/using-widevine-cdm-plugin.md)
* [Offscreen Rendering](tutorial/offscreen-rendering.md)

* * *

* [Glossary of Terms](glossary.md)

## API References

* [Synopsis](api/synopsis.md)
* [Process Object](api/process.md)
* [Supported Chrome Command Line Switches](api/chrome-command-line-switches.md)
* [Environment Variables](api/environment-variables.md)
* [Breaking API Changes](api/breaking-changes.md)

### Custom DOM Elements:

* [`File` Object](api/file-object.md)
* [`<webview>` Tag](api/webview-tag.md)
* [`window.open` Function](api/window-open.md)

### Modules for the Main Process:

* [app](api/app.md)
* [autoUpdater](api/auto-updater.md)
* [BrowserView](api/browser-view.md)
* [BrowserWindow](api/browser-window.md)
* [contentTracing](api/content-tracing.md)
* [dialog](api/dialog.md)
* [globalShortcut](api/global-shortcut.md)
* [inAppPurchase](api/in-app-purchase.md)
* [ipcMain](api/ipc-main.md)
* [Menu](api/menu.md)
* [MenuItem](api/menu-item.md)
* [net](api/net.md)
* [netLog](api/netLog.md)
* [powerMonitor](api/power-monitor.md)
* [powerSaveBlocker](api/power-save-blocker.md)
* [protocol](api/protocol.md)
* [session](api/session.md)
* [systemPreferences](api/system-preferences.md)
* [Tray](api/tray.md)
* [webContents](api/web-contents.md)

### Modules for the Renderer Process (Web Page):

* [desktopCapturer](api/desktop-capturer.md)
* [ipcRenderer](api/ipc-renderer.md)
* [remote](api/remote.md)
* [webFrame](api/web-frame.md)

### Modules for Both Processes:

* [clipboard](api/clipboard.md)
* [crashReporter](api/crash-reporter.md)
* [nativeImage](api/native-image.md)
* [screen](api/screen.md)
* [shell](api/shell.md)

## توسعه

See <development/README.md>