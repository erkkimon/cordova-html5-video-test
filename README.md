cordova-html5-video-test
========================

Making video tag work in a hybrid app can be pure pain because there are so many variables. That's why this demo was created. This repo should compile fine with Cordova, and the result should work in Android 4.1. At the moment, there's no success with Android 4.4, so feel free to share your ideas or to leave a pull request. 
  
For Android 4.1, this repo provides:
  - correctly encoded video files with needed ffmpeg arguments
  - correctly formed html5 video tag
  - correct reference to video files, and 
  - correct set of video tag attributes (= no type).

# Tests

These tests have been performed on 2014-09-07 14–15 EEST 2014.

---

## Android 4.1

**Summary:** The video works and autoplays. All the videos play inline. The videos play again, when the play button is being tapped.

### Version info

- cordova-html5-video-test: 1daba8170ba1196d54c8ea663225424e0bc6b6d0
- Cordova: 3.5.0-0.2.4
- NodeJS: v0.10.29
- npm: 1.4.16
- Android: 4.1.1
- Android SDK: 18
- Device: HUAWEI G510-0200

### Log

The log includes launch event (cordova run) and a play-tap on every video.

### Remote Inspector Log

*N/A*

### ADB Log

```
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/NetworkManagementSocketTagger(23313): untagSocket(101) failed with errno -22
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/dalvikvm(23313): GC_CONCURRENT freed 1008K, 20% free 11035K/13699K, paused 12ms+21ms, total 96ms
E/dalvikvm(23313): GC_CONCURRENT freed 897K, 19% free 11211K/13699K, paused 13ms+24ms, total 96ms
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
W/NetworkManagementSocketTagger(23313): untagSocket(101) failed with errno -22
E/dalvikvm(23313): GC_EXPLICIT freed 1563K, 25% free 10405K/13699K, paused 10ms+5ms, total 59ms
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
I/PeopleSync(23313): Sync finished, successful=true, took 124711ms
I/PeopleSync(23313): Sync start: cannotHavePeople=false isPageExistenceCheckOnly=false
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
W/NetworkManagementSocketTagger(23313): untagSocket(101) failed with errno -22
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/NetworkManagementSocketTagger(23313): untagSocket(101) failed with errno -22
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
W/NetworkManagementSocketTagger(23313): untagSocket(101) failed with errno -22
I/PeopleSync(23313): Sync finished, successful=true, took 2257ms
I/PeopleSync(23313): Sync finished, duration: 127206 [b847012a]
E/Trace   (24751): error opening trace file: No such file or directory (2)
W/dalvikvm(24751): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
I/ActivityThread(24751): Pub com.android.browser;browser: com.android.browser.provider.BrowserProvider2
I/ActivityThread(24751): Pub com.android.browser.home: com.android.browser.homepages.HomeProvider
I/ActivityThread(24751): Pub com.android.browser.snapshots: com.android.browser.provider.SnapshotProvider
E/BrowserSettings(24751): Error while trying to get homepage from browser_config
E/BrowserSettings(24751): java.io.FileNotFoundException: /data/cust/xml/browser_config.xml: open failed: ENOENT (No such file or directory)
E/BrowserSettings(24751):   at libcore.io.IoBridge.open(IoBridge.java:416)
E/BrowserSettings(24751):   at java.io.FileInputStream.<init>(FileInputStream.java:78)
E/BrowserSettings(24751):   at java.io.FileInputStream.<init>(FileInputStream.java:105)
E/BrowserSettings(24751):   at com.android.browser.BrowserSettings$1.run(BrowserSettings.java:368)
E/BrowserSettings(24751):   at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1076)
E/BrowserSettings(24751):   at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:569)
E/BrowserSettings(24751):   at java.lang.Thread.run(Thread.java:856)
E/BrowserSettings(24751): Caused by: libcore.io.ErrnoException: open failed: ENOENT (No such file or directory)
E/BrowserSettings(24751):   at libcore.io.Posix.open(Native Method)
E/BrowserSettings(24751):   at libcore.io.BlockGuardOs.open(BlockGuardOs.java:110)
E/BrowserSettings(24751):   at libcore.io.IoBridge.open(IoBridge.java:400)
E/BrowserSettings(24751):   ... 6 more
W/System.err(24751): Invalid int: ""
E/SQLiteLog(24751): (5) statement aborts at 1: [PRAGMA journal_mode=TRUNCATE;]
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/Trace   (24771): error opening trace file: No such file or directory (2)
W/dalvikvm(24771): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
I/ActivityThread(24771): Pub com.google.android.gm2.accountcache: com.android.mail.providers.GmailAccountCacheProvider
I/ActivityThread(24771): Pub gmail-ls: com.google.android.gm.provider.MailProvider
W/System.err(24771): Invalid int: ""
I/ActivityThread(24771): Pub com.google.android.gm: com.google.android.gm.provider.PublicContentProvider
I/ActivityThread(24771): Pub com.google.android.gmail.SuggestionsProvider: com.google.android.gm.SuggestionsProvider
I/ActivityThread(24771): Pub com.google.android.gm2.conversation.provider: com.android.mail.browse.GmailConversationProvider
I/ActivityThread(24771): Pub com.android.gmail.ui: com.google.android.gm.provider.UiProvider
I/GmsClient(24771): connect: bindService returned true for Intent { act=com.google.android.gms.icing.INDEX_SERVICE }
E/dalvikvm(  455): GC_EXPLICIT freed 1888K, 43% free 16083K/27847K, paused 22ms+14ms, total 157ms
E/SQLiteLog(24771): (5) statement aborts at 1: [PRAGMA journal_mode=TRUNCATE;]
I/Gmail   (24771): calculateUnknownSyncRationalesAndPurgeInBackground: queueing
E/SQLiteLog(24771): (5) statement aborts at 1: [PRAGMA journal_mode=TRUNCATE;]
I/Gmail   (24771): calculateUnknownSyncRationalesAndPurgeInBackground: queueing
I/Gmail   (24771): MainSyncRequestProto: lowestBkwdConvoId: 0, highestHandledServerOp: 3606718, normalSync: true
I/Gmail   (24771): calculateUnknownSyncRationalesAndPurgeInBackground: running
I/Gmail   (24771): calculateUnknownSyncRationalesAndPurgeInBackground: running
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/dalvikvm(24771): GC_EXPLICIT freed 1648K, 36% free 8801K/13699K, paused 5ms+6ms, total 70ms
I/Gmail   (24771): MainSyncRequestProto: lowestBkwdConvoId: 0, highestHandledServerOp: 3606723, normalSync: true
I/Gmail   (24771): lowestBackward conversation id 0
/GmsClient(24771): connect: bindService returned true for Intent { act=com.google.android.gms.icing.INDEX_SERVICE }
E/Trace   (24815): error opening trace file: No such file or directory (2)
W/dalvikvm(24815): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
W/System.err(24815): Invalid int: ""
E/Qcom_fm_if.c(24832): find the id:libqcomfm_if and begins to open the devices
E/android_hardware_fm.cpp(24832): register_android_hardware_fm_fmradio, ret is 0
E/Trace   (24845): error opening trace file: No such file or directory (2)
W/dalvikvm(24845): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
I/PackageParser(  455): add hwframework.jar as a optional shared library.
I/PackageManager(  455): Removing non-system package:com.video.test
I/PackageManager(  455): Running dexopt on: com.video.test
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
E/dalvikvm(  772): GC_EXPLICIT freed 828K, 31% free 11787K/16967K, paused 5ms+4ms, total 86ms
E/dalvikvm( 6060): GC_EXPLICIT freed 319K, 36% free 8797K/13699K, paused 3ms+3ms, total 75ms
E/dalvikvm( 5931): GC_EXPLICIT freed 1001K, 17% free 16502K/19655K, paused 4ms+10ms, total 81ms
I/ApplicationsProvider( 6060): sendGCMsg()
E/HwTransition( 5931): TERR: No drawchild is invoked, let launcher do the draw 0.0
E/dalvikvm(  455): GC_EXPLICIT freed 1512K, 43% free 16127K/27847K, paused 15ms+14ms, total 195ms
E/Trace   (24866): error opening trace file: No such file or directory (2)
W/ResourceType(  455): Failure getting entry for 0x7f080000 (t=7 e=0) in package 0 (error -75)
W/ResourceType(  455): Failure getting entry for 0x7f080000 (t=7 e=0) in package 0 (error -75)
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
E/dalvikvm(  455): GC_EXPLICIT freed 141K, 43% free 16064K/27847K, paused 18ms+13ms, total 199ms
W/dalvikvm(24866): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
E/dalvikvm(24832): GC_CONCURRENT freed 100K, 82% free 483K/2560K, paused 1ms+0ms, total 4ms
I/ActivityThread(24866): Pub com.android.gallery3d.provider: com.android.gallery3d.provider.GalleryProvider
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/Trace   (24891): error opening trace file: No such file or directory (2)
W/dalvikvm(24891): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
E/Trace   (24904): error opening trace file: No such file or directory (2)
E/dalvikvm(  155): GC_EXPLICIT freed 38K, 42% free 7998K/13699K, paused 2ms+2ms, total 41ms
W/dalvikvm(24904): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
E/dalvikvm(  155): GC_EXPLICIT freed <1K, 42% free 7998K/13699K, paused 1ms+1ms, total 27ms
E/dalvikvm(  155): GC_EXPLICIT freed <1K, 42% free 7998K/13699K, paused 2ms+2ms, total 40ms
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/Trace   (24926): error opening trace file: No such file or directory (2)
W/dalvikvm(24926): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
W/System.err(24891): Invalid int: ""
I/ActivityThread(24926): Pub com.google.android.finsky.QSBSuggestionsProvider2: com.google.android.finsky.providers.QSBSuggestionsProvider
I/ActivityThread(24926): Pub com.google.android.finsky.AppIconProvider: com.google.android.finsky.providers.AppIconProvider
I/ActivityThread(24926): Pub com.google.android.finsky.RecentSuggestionsProvider: com.google.android.finsky.providers.RecentSuggestionsProvider
W/System.err(24926): Invalid int: ""
E/Qcom_fm_if.c(24890): find the id:libqcomfm_if and begins to open the devices
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
E/android_hardware_fm.cpp(24890): register_android_hardware_fm_fmradio, ret is 0
I/Input   (24890): InjectKeyEvent: KeyEvent { action=ACTION_DOWN, keyCode=KEYCODE_MENU, scanCode=0, metaState=0, flags=0x0, repeatCount=0, eventTime=310707278, downTime=310707278, deviceId=-1, source=0x101 }
W/WindowManager(  455): statePower =normal
E/WindowManager(  455): getkey down, keyCode =true, 82
W/lights  (  455): TP Button Light current value is 255
W/lights  (  455): button_backlight:property_get,percent =50
I/Input   (24890): InjectKeyEvent: KeyEvent { action=ACTION_UP, keyCode=KEYCODE_MENU, scanCode=0, metaState=0, flags=0x0, repeatCount=0, eventTime=310707278, downTime=310707278, deviceId=-1, source=0x101 }
W/WindowManager(  455): statePower =normal
E/WindowManager(  455): getkey down, keyCode =false, 82
E/dalvikvm(24890): GC_CONCURRENT freed 102K, 82% free 479K/2560K, paused 1ms+1ms, total 5ms
W/dalvikvm(24926): VFY: unable to resolve static method 896: Landroid/provider/Settings$Global;.getInt (Landroid/content/ContentResolver;Ljava/lang/String;I)I
W/dalvikvm(24926): VFY: unable to resolve static method 896: Landroid/provider/Settings$Global;.getInt (Landroid/content/ContentResolver;Ljava/lang/String;I)I
W/dalvikvm(24926): VFY: unable to resolve virtual method 863: Landroid/os/StatFs;.getAvailableBytes ()J
W/dalvikvm(24926): VFY: unable to resolve virtual method 387: Landroid/content/pm/PackageManager;.extendVerificationTimeout (IIJ)V
E/dalvikvm(24154): GC_EXPLICIT freed 561K, 40% free 8249K/13699K, paused 5ms+5ms, total 90ms
E/dalvikvm( 9523): GC_EXPLICIT freed 821K, 19% free 11163K/13699K, paused 3ms+7ms, total 111ms
I/GoogleHttpClient(23313): Falling back to old SSLCertificateSocketFactory
E/Trace   (24969): error opening trace file: No such file or directory (2)
W/dalvikvm(24969): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
E/dalvikvm(  455): GC_EXPLICIT freed 1002K, 42% free 16168K/27847K, paused 5ms+17ms, total 212ms
E/dalvikvm(24815): GC_CONCURRENT freed 4691K, 39% free 8417K/13699K, paused 18ms+8ms, total 225ms
I/MultiDex(24969): install
I/MultiDex(24969): MultiDexExtractor.load(/data/app/com.google.android.gms-1.apk, false)
I/MultiDex(24969): loading existing secondary dex files
I/MultiDex(24969): load found 1 secondary dex files
E/Qcom_fm_if.c(24964): find the id:libqcomfm_if and begins to open the devices
I/ApplicationsProvider( 6060): System.gc()
I/MultiDex(24969): install done
I/ActivityThread(24969): Pub com.google.android.gms.drive: com.google.android.gms.drive.data.sync.syncadapter.DatabaseNotificationContentProvider
E/android_hardware_fm.cpp(24964): register_android_hardware_fm_fmradio, ret is 0
E/dalvikvm( 6060): GC_EXPLICIT freed 286K, 36% free 8815K/13699K, paused 10ms+5ms, total 165ms
I/ProviderInstaller(24969): Insert disabled by gate 'gms:security:enable_conscrypt_in_gms_application'
E/Trace   (24991): error opening trace file: No such file or directory (2)
W/dalvikvm(24991): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
I/CordovaLog(24991): Changing log level to DEBUG(3)
I/CordovaLog(24991): Found start page location: index.html
W/dalvikvm(24991): VFY: unable to resolve static method 2333: Lorg/apache/cordova/CordovaWebView;.setWebContentsDebuggingEnabled (Z)V
E/dalvikvm(24815): GC_EXPLICIT freed 437K, 39% free 8391K/13699K, paused 266ms+17ms, total 418ms
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/lights  (  455): TP Button Light current value is 0
W/lights  (  455): button_backlight:property_get,percent =50
E/dalvikvm(24154): GC_EXPLICIT freed 235K, 41% free 8217K/13699K, paused 9ms+6ms, total 56ms
E/Trace   (25012): error opening trace file: No such file or directory (2)
W/dalvikvm(25012): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
I/ActivityThread(25012): Pub com.svox.pico.providers.SettingsProvider: com.svox.pico.providers.SettingsProvider
E/WeatherApp(24661): WeatherApp+mydebuglog+KillProcess
I/CordovaWebView(24991): Disabled addJavascriptInterface() bridge since Android version is old.
W/System.err(24991): Invalid int: ""
I/CordovaLog(24991): Changing log level to DEBUG(3)
I/CordovaLog(24991): Found start page location: index.html
I/Adreno200-EGL(24991): <qeglDrvAPI_eglInitialize:299>: EGL 1.4 QUALCOMM build: AU_LINUX_ANDROID_JB_REL_2.0.3.04.01.01.21.010_msm8625_JB_REL_2.0.3_Merge_release_AU (Merge)
I/Adreno200-EGL(24991): Build Date: 10/26/12 Fri
I/Adreno200-EGL(24991): Local Branch:
I/Adreno200-EGL(24991): Remote Branch: quic/jb_rel_2.0.3
I/Adreno200-EGL(24991): Local Patches: NONE
I/Adreno200-EGL(24991): Reconstruct Branch: AU_LINUX_ANDROID_JB_REL_2.0.3.04.01.01.21.010 +  NOTHING
E/dalvikvm(  455): GC_EXPLICIT freed 700K, 44% free 15844K/27847K, paused 19ms+9ms, total 181ms
E/dalvikvm(24154): GC_EXPLICIT freed 193K, 40% free 8277K/13699K, paused 2ms+31ms, total 86ms
I/ActivityManager(  455): Displayed com.video.test/.VideoTest: +1s754ms
E/dalvikvm(24964): GC_CONCURRENT freed 102K, 80% free 518K/2560K, paused 1ms+1ms, total 6ms
E/MediaPlayer(24991): Uri is  android.resource://com.video.test/raw/mp4video
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 5
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
E/MM_OSAL (30180): ValidateAACFile failed
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
E/HwDevCtlService(  154): setCABCMode ret is 0
E/MediaPlayer(24991): Uri is  android.resource://com.video.test/raw/webmvideo
E/omx_vdec(30180): m_enable_android_native_buffers 1
W/MemoryDealer(30180): madvise(0x41a99000, 327680, MADV_REMOVE) returned Operation not supported on transport endpoint
W/MemoryDealer(30180): madvise(0x41a99000, 327680, MADV_REMOVE) returned Operation not supported on transport endpoint
E/omx_vdec(30180): get_parameter: OMX_GoogleAndroidIndexGetAndroidNativeBufferUsage
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 29, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 34, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 38, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 42, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 48, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 52, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 56, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 47, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 63, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/OMXCodec(30180): failed to allocate node OMX.qcom.video.decoder.vp8
E/MediaPlayer(24991): Uri is  android.resource://com.video.test/raw/mp4video
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 68, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 74, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 78, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 82, size = 94208
E/omx_vdec(30180): using android_native_buffers
E/omx_vdec(30180): Extension: OMX.google.android.index.useAndroidNativeBuffer2 is not supported
E/omx_vdec(30180): Inside use_android_native_buffer
E/omx_vdec(30180): mmaping pmem with fd = 86, size = 94208
E/omx_vdec(30180): using android_native_buffers
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 5
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
E/MM_OSAL (30180): ValidateAACFile failed
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
W/QComExtractorFactory(30180): Didn't match the sniff <=== status = 1
E/omx_vdec(30180): Video decoder instance already exists.
E/OMXCodec(30180): failed to allocate node OMX.qcom.video.decoder.avc
E/MediaPlayer(24991): Uri is  android.resource://com.video.test/raw/webmvideo
E/ITTIAM_OMX_VDEC(30180): Unsupported resolution width 320: height 176
E/OMXCodec(30180): failed to allocate node OMX.qcom.video.decoder.vp8
W/OMXCodec(30180): Failed to set frame packing format on component
E/omx_vdec(30180): Set the VDEC_YAMATO_DISPLAY_FORMAT Color Format
E/omx_vdec(30180): Set the VDEC_YAMATO_DISPLAY_FORMAT Color Format
E/vdec    (30180): allocating pmem for input only - usebuffer case
E/vdec    (30180): Calling vdec_pmem_alloc
E/vdec_pmem(30180): ION_mem_alloc1 called with size 2621440
E/vdec_pmem(30180): Open /dev/ion with options 4096, base =0x43d11000, fd 101
E/        (30180):
E/        (30180):  SetParameter, Setting display format to Yamato
E/        (30180): SPS: Decode: old WxH = 320x176,new WxH = 320x176
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x43308190 successful
W/MemoryDealer(30180): madvise(0x42f9f000, 114688, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x433083a0 successful
W/MemoryDealer(30180): madvise(0x42fbc000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x41f1b528 successful
W/MemoryDealer(30180): madvise(0x42fd8000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x41f1b668 successful
W/MemoryDealer(30180): madvise(0x42ff4000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x42353850 successful
W/MemoryDealer(30180): madvise(0x426a6000, 114688, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x40050c38 successful
W/MemoryDealer(30180): madvise(0x426c3000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x41bab828 successful
W/MemoryDealer(30180): madvise(0x426df000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x403c8a78 successful
W/MemoryDealer(30180): madvise(0x426fb000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/vdl     (30180): registering the PMEM buffers for index 0 fd 29 and base 0x41d53000
E/vdl     (30180): registering the PMEM buffers for index 1 fd 34 and base 0x41d6a000
E/vdl     (30180): registering the PMEM buffers for index 2 fd 38 and base 0x41d85000
E/vdl     (30180): registering the PMEM buffers for index 3 fd 42 and base 0x4203e000
E/vdl     (30180): registering the PMEM buffers for index 4 fd 48 and base 0x42055000
E/vdl     (30180): registering the PMEM buffers for index 5 fd 52 and base 0x4206c000
E/vdl     (30180): registering the PMEM buffers for index 6 fd 56 and base 0x42083000
E/vdl     (30180): registering the PMEM buffers for index 7 fd 47 and base 0x420b1000
E/vdl     (30180): registering the PMEM buffers for index 8 fd 63 and base 0x42100000
E/vdl     (30180): registering the PMEM buffers for index 9 fd 68 and base 0x422f5000
E/vdl     (30180): registering the PMEM buffers for index 10 fd 74 and base 0x42323000
E/vdl     (30180): registering the PMEM buffers for index 11 fd 78 and base 0x4233a000
E/vdl     (30180): registering the PMEM buffers for index 12 fd 82 and base 0x4265d000
E/vdl     (30180): registering the PMEM buffers for index 13 fd 86 and base 0x42674000
E/vdec_pmem(30180): ION_mem_alloc1 called with size 221760
E/vdec_pmem(30180): Open /dev/ion with options 4096, base =0x426a6000, fd 103
E/VDL_RTOS(30180): ***YAMATO Enabled***
E/VDL_RTOS(30180): Flush VDL_stats_q: stats_ptr 0x41f17b50
E/omx_vdec(30180): Warning - previous ts > current ts. And both are non B-frames
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x4004e0a0 successful
W/MemoryDealer(30180): madvise(0x41d9c000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x42443090 successful
W/MemoryDealer(30180): madvise(0x41d9e000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x4212d178 successful
W/MemoryDealer(30180): madvise(0x41da0000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x40875c80 successful
W/MemoryDealer(30180): madvise(0x41da2000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x403c6de8 successful
W/MemoryDealer(30180): madvise(0x4297b000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x43b10f18 successful
W/MemoryDealer(30180): madvise(0x42983000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x430886c8 successful
W/MemoryDealer(30180): madvise(0x4298b000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x41f20368 successful
W/MemoryDealer(30180): madvise(0x42993000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x420cbaf0 successful
W/MemoryDealer(30180): madvise(0x4299b000, 114688, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x43309e78 successful
W/MemoryDealer(30180): madvise(0x429b8000, 110592, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x410564c8 successful
W/MemoryDealer(30180): madvise(0x429d4000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x420d14d0 successful
W/MemoryDealer(30180): madvise(0x429dc000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x420d1610 successful
W/MemoryDealer(30180): madvise(0x429e4000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x420d1738 successful
W/MemoryDealer(30180): madvise(0x429ec000, 32768, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x433071d8 successful
W/MemoryDealer(30180): madvise(0x42359000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x403b9c00 successful
W/MemoryDealer(30180): madvise(0x4235b000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x403b9d40 successful
W/MemoryDealer(30180): madvise(0x4235d000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/OMXNodeInstance(30180): OMX_FreeBuffer for buffer header 0x403b9e68 successful
W/MemoryDealer(30180): madvise(0x4235f000, 8192, MADV_REMOVE) returned Operation not supported on transport endpoint
E/Trace   (25080): error opening trace file: No such file or directory (2)
I/PeopleContactsSync(23313): CP2 sync disabled
W/dalvikvm(25080): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/Trace   (25094): error opening trace file: No such file or directory (2)
W/dalvikvm(25094): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
I/PeopleContactsSync(23313): CP2 sync disabled
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/Trace   (25114): error opening trace file: No such file or directory (2)
W/dalvikvm(25114): Refusing to reopen boot DEX '/system/framework/hwframework.jar'
I/PowerSavingService(  772): The battery low alert is already alerted.
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/dalvikvm(24815): GC_EXPLICIT freed 421K, 38% free 8542K/13699K, paused 75ms+817ms, total 1729ms
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
E/dalvikvm(24154): GC_EXPLICIT freed 264K, 39% free 8423K/13699K, paused 9ms+5ms, total 211ms
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/dalvikvm(  455): GC_EXPLICIT freed 725K, 44% free 15850K/27847K, paused 9ms+20ms, total 228ms
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/lights  (  455): TP Button Light current value is 255
W/lights  (  455): button_backlight:property_get,percent =50
E/VDL_RTOS(30180): Flush VDL_stats_q: stats_ptr 0x0
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/dalvikvm(24154): GC_CONCURRENT freed 1490K, 39% free 8493K/13699K, paused 15ms+26ms, total 90ms
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/dalvikvm(24154): GC_EXPLICIT freed 389K, 41% free 8148K/13699K, paused 8ms+11ms, total 58ms
W/GLSUser ( 9523): GoogleAccountDataService.getToken()
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/lights  (  455): TP Button Light current value is 0
W/lights  (  455): button_backlight:property_get,percent =50
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
E/WifiHW  (  455): wifi_send_command : SIGNAL_POLL ; interface index=0;
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
W/SignalStrength(  772): getLTELevel - rsrp:2147483647 snr:2147483647 rsrpIconLevel:-1 snrIconLevel:-1
W/SignalStrength(  772): getLTELevel - rssi:99 rssiIconLevel:0
W/SignalStrength(  772): getGsmLevel=3
W/SignalStrength(  772): getLevel=3
```

---
    
## Android 4.4

**Summary:** Not any of the videos autoplays. Even tapping the play button doesn't start playback. The videos don't seem to load at all, because only video symbol is being shown in the positions the videos should be loaded to. 

### Version info

- cordova-html5-video-test: 1daba8170ba1196d54c8ea663225424e0bc6b6d0
- Cordova: 3.5.0-0.2.4
- NodeJS: v0.10.29
- npm: 1.4.16
- Android: 4.4.2
- Android SDK: 18
- Device: Samsung Galaxy S2 GT-L9100

### Log

The log includes launch event (cordova run) and a play-tap on every video.

### Remote Inspector Log

```
Viewport target-densitydpi is not supported. index.html:6
Failed to load resource android.resource://com.video.test/raw/mp4video
Failed to load resource android.resource://com.video.test/raw/webmvideo
Failed to load resource android.resource://com.video.test/raw/mp4video
Failed to load resource android.resource://com.video.test/raw/webmvideo
```

### ADB Log

```
D/AndroidRuntime(20033):
D/AndroidRuntime(20033): >>>>>> AndroidRuntime START com.android.internal.os.RuntimeInit <<<<<<
D/AndroidRuntime(20033): CheckJNI is OFF
D/dalvikvm(20033): Trying to load lib libjavacore.so 0x0
D/dalvikvm(20033): Added shared lib libjavacore.so 0x0
D/dalvikvm(20033): Trying to load lib libnativehelper.so 0x0
D/dalvikvm(20033): Added shared lib libnativehelper.so 0x0
D/dalvikvm(20033): No JNI_OnLoad found in libnativehelper.so 0x0, skipping init
E/cutils-trace(20033): Error opening trace file: No such file or directory (2)
D/dalvikvm(20033): Note: class Landroid/app/ActivityManagerNative; has 180 unimplemented (abstract) methods
E/memtrack(20033): Couldn't load memtrack module (No such file or directory)
E/android.os.Debug(20033): failed to load memtrack module: -2
D/AndroidRuntime(20033): Calling main entry com.android.commands.pm.Pm
V/Zygote  (20049): Switching descriptor 31 to /dev/null
V/Zygote  (20049): Switching descriptor 10 to /dev/null
I/ActivityManager( 2263): Start proc com.android.defcontainer for service com.android.defcontainer/.DefaultContainerService: pid=20049 uid=10003 gids={50003, 1028, 1015, 1023, 2001, 1035}
W/ActivityManager( 2263): No content provider found for permission revoke: file:///data/local/tmp/VideoTest-debug-unaligned.apk
W/ActivityManager( 2263): No content provider found for permission revoke: file:///data/local/tmp/VideoTest-debug-unaligned.apk
I/PackageManager( 2263): Copying native libraries to /data/app-lib/vmdl1276150343
I/ActivityManager( 2263): Force stopping com.video.test appid=10060 user=-1: uninstall pkg
I/ActivityManager( 2263): Killing 10185:com.video.test/u0a60 (adj 7): stop com.video.test
I/ActivityManager( 2263):   Force finishing activity ActivityRecord{4242a068 u0 com.video.test/.VideoTest t20}
I/WindowState( 2263): WIN DEATH: Window{42a07190 u0 com.video.test/com.video.test.VideoTest}
I/PackageManager( 2263): Package com.video.test codePath changed from /data/app/com.video.test-1.apk to /data/app/com.video.test-2.apk; Retaining data and using new
I/PackageManager( 2263): Running dexopt on: com.video.test
D/dalvikvm(20065): DexOpt: load 31ms, verify+opt 281ms, 727948 bytes
I/ActivityManager( 2263): Force stopping com.video.test appid=10060 user=-1: update pkg
W/PackageManager( 2263): Code path for pkg : com.video.test changing from /data/app/com.video.test-1.apk to /data/app/com.video.test-2.apk
W/PackageManager( 2263): Resource path for pkg : com.video.test changing from /data/app/com.video.test-1.apk to /data/app/com.video.test-2.apk
I/ActivityManager( 2263): Force stopping com.video.test appid=10060 user=0: pkg removed
I/InputReader( 2263): Reconfiguring input devices.  changes=0x00000010
V/Zygote  (20069): Switching descriptor 31 to /dev/null
V/Zygote  (20069): Switching descriptor 10 to /dev/null
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "sms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/ActivityManager( 2263): Start proc com.android.vending for broadcast com.android.vending/com.google.android.finsky.receivers.PackageMonitorReceiver$RegisteredReceiver: pid=20069 uid=10019 gids={50019, 3003, 1028, 1015, 1023}
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "smsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mmsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "sms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "smsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
D/BackupManagerService( 2263): Received broadcast Intent { act=android.intent.action.PACKAGE_REMOVED dat=package:com.video.test flg=0x4000010 (has extras) }
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mmsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/InputReader( 2263): Reconfiguring input devices.  changes=0x00000010
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "sms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
D/BackupManagerService( 2263): Received broadcast Intent { act=android.intent.action.PACKAGE_ADDED dat=package:com.video.test flg=0x4000010 (has extras) }
V/BackupManagerService( 2263): removePackageParticipantsLocked: uid=10060 #1
V/BackupManagerService( 2263): addPackageParticipantsLocked: #1
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "smsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/InputReader( 2263): Reconfiguring input devices.  changes=0x00000010
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mmsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "sms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "smsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mmsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "sms"
D/Finsky  (20069): [1] FinskyApp.onCreate: Initializing network with DFE https://android.clients.google.com/fdfe/
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
D/AndroidRuntime(20033): Shutting down VM
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "smsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mmsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "sms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "smsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mms"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
I/PackageManager( 2263):   Action: "android.intent.action.SENDTO"
I/PackageManager( 2263):   Category: "android.intent.category.DEFAULT"
I/PackageManager( 2263):   Scheme: "mmsto"
I/PackageManager( 2263): Adding preferred activity ComponentInfo{com.android.mms/com.android.mms.ui.ComposeMessageActivity} for user 0 :
D/Finsky  (20069): [1] DailyHygiene.goMakeHygieneIfDirty: No need to run daily hygiene.
W/Settings(20069): Setting download_manager_max_bytes_over_mobile has moved from android.provider.Settings.Secure to android.provider.Settings.Global.
W/Settings(20069): Setting download_manager_recommended_max_bytes_over_mobile has moved from android.provider.Settings.Secure to android.provider.Settings.Global.
D/Finsky  (20069): [1] GmsCoreHelper.cleanupNlp: result=false type=4
I/ActivityManager( 2263): Start proc com.android.keychain for broadcast com.android.keychain/.KeyChainBroadcastReceiver: pid=20111 uid=1000 gids={41000, 1028, 1015, 1023, 3002, 3001, 3003}
D/Finsky  (20069): [1] 2.run: Loaded library for account: [XL9_RlY4vJVW37KxjdwtW45Ftkk]
D/Finsky  (20069): [1] 2.run: Finished loading 1 libraries.
D/Finsky  (20069): [1] RestoreTracker.stopServiceIfDone: Restore complete with 0 success and 0 failed.
W/Searchables( 2263): No global search activity found
W/Searchables( 2263): No global search activity found
W/RecognitionManagerService( 2263): no available voice recognition services found for user 0
V/Zygote  (20111): Switching descriptor 31 to /dev/null
V/Zygote  (20111): Switching descriptor 10 to /dev/null
W/ContextImpl(20111): Calling a method in the system process without a qualified user: android.app.ContextImpl.startService:1479 android.content.ContextWrapper.startService:494 android.content.ContextWrapper.startService:494 com.android.keychain.KeyChainBroadcastReceiver.onReceive:12 android.app.ActivityThread.handleReceiver:2422
V/Zygote  (20126): Switching descriptor 31 to /dev/null
V/Zygote  (20126): Switching descriptor 10 to /dev/null
I/ActivityManager( 2263): Start proc com.android.gallery3d for broadcast com.android.gallery3d/.app.PackagesMonitor: pid=20126 uid=10033 gids={50033, 3003, 1028, 1015, 1023}
D/AndroidRuntime(20109):
D/AndroidRuntime(20109): >>>>>> AndroidRuntime START com.android.internal.os.RuntimeInit <<<<<<
D/AndroidRuntime(20109): CheckJNI is OFF
D/dalvikvm(20109): Trying to load lib libjavacore.so 0x0
D/dalvikvm(20109): Added shared lib libjavacore.so 0x0
D/dalvikvm(20109): Trying to load lib libnativehelper.so 0x0
D/dalvikvm(20109): Added shared lib libnativehelper.so 0x0
D/dalvikvm(20109): No JNI_OnLoad found in libnativehelper.so 0x0, skipping init
E/cutils-trace(20109): Error opening trace file: No such file or directory (2)
D/dalvikvm(20109): Note: class Landroid/app/ActivityManagerNative; has 180 unimplemented (abstract) methods
E/memtrack(20109): Couldn't load memtrack module (No such file or directory)
E/android.os.Debug(20109): failed to load memtrack module: -2
V/Zygote  (20149): Switching descriptor 31 to /dev/null
V/Zygote  (20149): Switching descriptor 10 to /dev/null
I/ActivityManager( 2263): Start proc com.google.android.gms.drive for broadcast com.google.android.gms/.drive.api.DriveSystemBroadcastReceiver: pid=20149 uid=10014 gids={50014, 3003, 1007, 1028, 1023, 1015, 3002, 3001, 3007, 2001, 3006}
D/PackageBroadcastService(17639): Received broadcast action=android.intent.action.PACKAGE_REMOVED and uri=com.video.test
D/AndroidRuntime(20109): Calling main entry com.android.commands.input.Input
I/Input   (20109): injectKeyEvent: KeyEvent { action=ACTION_DOWN, keyCode=KEYCODE_MENU, scanCode=0, metaState=0, flags=0x0, repeatCount=0, eventTime=14712035, downTime=14712035, deviceId=-1, source=0x101 }
I/MultiDex(20149): install
I/MultiDex(20149): MultiDexExtractor.load(/data/app/com.google.android.gms-1.apk, false)
D/lights  ( 2263): set_light_buttons: 1
I/Input   (20109): injectKeyEvent: KeyEvent { action=ACTION_UP, keyCode=KEYCODE_MENU, scanCode=0, metaState=0, flags=0x0, repeatCount=0, eventTime=14712035, downTime=14712035, deviceId=-1, source=0x101 }
I/MultiDex(20149): loading existing secondary dex files
I/MultiDex(20149): load found 1 secondary dex files
D/AndroidRuntime(20109): Shutting down VM
W/AudioTrack( 2263): AUDIO_OUTPUT_FLAG_FAST denied by client due to mismatching sample rate (48000 vs 44100)
D/Yamaha-MC1N2-Audio( 1849): yamaha_mc1n2_audio_output_start()
D/Yamaha-MC1N2-Audio( 1849): yamaha_mc1n2_audio_route_start()
D/Yamaha-MC1N2-Audio( 1849): (yamaha_mc1n2_audio_params_route_find): device = 2, direction = 0
I/MultiDex(20149): install done
I/ProviderInstaller(20149): Insert disabled by gate 'gms:security:enable_conscrypt_in_gms_application'
V/Zygote  (20169): Switching descriptor 31 to /dev/null
V/Zygote  (20169): Switching descriptor 10 to /dev/null
I/ActivityManager( 2263): Start proc com.google.android.partnersetup for broadcast com.google.android.partnersetup/.RlzPingBroadcastReceiver: pid=20169 uid=10017 gids={50017, 3003}
D/PackageAddedReceiver(17621): package added com.video.test
D/PackageBroadcastService(17639): Received broadcast action=android.intent.action.PACKAGE_ADDED and uri=com.video.test
I/ActivityManager( 2263): Delay finish: com.google.android.gms/.wallet.receiver.PackageAddedBroadcastReceiver
I/ActivityManager( 2263): Resuming delayed broadcast
I/ActivityManager( 2263): Delay finish: com.google.android.gms/.app.receiver.SystemBroadcastReceiver
D/PackageBroadcastService(17639): Received broadcast action=android.intent.action.PACKAGE_REPLACED and uri=com.video.test
D/GCM     (17621): GcmService start Intent { act=com.google.android.gms.INITIALIZE flg=0x10 pkg=com.google.android.gms cmp=com.google.android.gms/.gcm.GcmService } com.google.android.gms.INITIALIZE
I/ActivityManager( 2263): Resuming delayed broadcast
I/PeopleContactsSync(17639): CP2 sync disabled
I/PeopleContactsSync(17639): CP2 sync disabled
D/AndroidRuntime(20193):
D/AndroidRuntime(20193): >>>>>> AndroidRuntime START com.android.internal.os.RuntimeInit <<<<<<
D/AndroidRuntime(20193): CheckJNI is OFF
D/dalvikvm(20193): Trying to load lib libjavacore.so 0x0
D/dalvikvm(20193): Added shared lib libjavacore.so 0x0
D/dalvikvm(20193): Trying to load lib libnativehelper.so 0x0
D/dalvikvm(20193): Added shared lib libnativehelper.so 0x0
D/dalvikvm(20193): No JNI_OnLoad found in libnativehelper.so 0x0, skipping init
D/dalvikvm(20193): Note: class Landroid/app/ActivityManagerNative; has 180 unimplemented (abstract) methods
E/cutils-trace(20193): Error opening trace file: No such file or directory (2)
E/memtrack(20193): Couldn't load memtrack module (No such file or directory)
E/android.os.Debug(20193): failed to load memtrack module: -2
D/AndroidRuntime(20193): Calling main entry com.android.commands.am.Am
I/ActivityManager( 2263): START u0 {act=android.intent.action.MAIN flg=0x10000000 cmp=com.video.test/.VideoTest} from pid 20193
V/Zygote  (20207): Switching descriptor 31 to /dev/null
V/Zygote  (20207): Switching descriptor 10 to /dev/null
D/dalvikvm(20207): Late-enabling CheckJNI
I/ActivityManager( 2263): Start proc com.video.test for activity com.video.test/.VideoTest: pid=20207 uid=10060 gids={50060, 3003}
I/healthd ( 1840): battery l=7 v=3772 t=28.0 h=2 st=2 c=0 chg=u
I/CordovaLog(20207): Changing log level to DEBUG(3)
I/CordovaLog(20207): Found start page location: index.html
D/Whitelist(20207): Unlimited access to network resources
D/CordovaActivity(20207): CordovaActivity.onCreate()
V/WebViewChromium(20207): Binding Chromium to the background looper Looper (main, tid 1) {42429e88}
I/chromium(20207): [INFO:library_loader_hooks.cc(112)] Chromium logging enabled: level = 0, default verbosity = 0
I/BrowserProcessMain(20207): Initializing chromium process, renderers=0
D/libEGL  (20207): loaded /system/lib/egl/libEGL_mali.so
D/libEGL  (20207): loaded /system/lib/egl/libGLESv1_CM_mali.so
D/libEGL  (20207): loaded /system/lib/egl/libGLESv2_mali.so
E/        (20207): Device driver API match
E/        (20207): Device driver API version: 23
E/        (20207): User space API version: 23
E/        (20207): mali: REVISION=Linux-r3p2-01rel3 BUILD_DATE=Wed Oct  9 21:05:57 KST 2013
W/chromium(20207): [WARNING:proxy_service.cc(888)] PAC support disabled because there is no system implementation
D/CordovaWebView(20207): CordovaWebView is running on device made by: samsung
D/JsMessageQueue(20207): Set native->JS mode to 2
D/CordovaActivity(20207): CordovaActivity.init()
D/CordovaWebView(20207): >>> loadUrl(file:///android_asset/www/index.html)
D/PluginManager(20207): init()
D/CordovaWebView(20207): >>> loadUrlNow()
I/CordovaLog(20207): Changing log level to DEBUG(3)
I/CordovaLog(20207): Found start page location: index.html
D/Whitelist(20207): Unlimited access to network resources
D/CordovaActivity(20207): Resuming the App
D/CordovaActivity(20207): CB-3064: The errorUrl is null
D/SoftKeyboardDetect(20207): Ignore this event
D/OpenGLRenderer(20207): Enabling debug mode 0
I/ActivityManager( 2263): Displayed com.video.test/.VideoTest: +1s89ms
I/ActivityManager( 2263): Timeline: Activity_windows_visible id: ActivityRecord{42ca44c8 u0 com.video.test/.VideoTest t22} time:14714121
D/SoftKeyboardDetect(20207): Ignore this event
D/AndroidRuntime(20193): Shutting down VM
I/ActivityManager(20207): Timeline: Activity_idle id: android.os.BinderProxy@4242bc68 time:14714138
D/CordovaWebViewClient(20207): onPageStarted(file:///android_asset/www/index.html)
D/CordovaActivity(20207): onMessage(onPageStarted,file:///android_asset/www/index.html)
D/CordovaLog(20207): file:///android_asset/www/index.html: Line 6 : Viewport target-densitydpi is not supported.
I/chromium(20207): [INFO:CONSOLE(6)] "Viewport target-densitydpi is not supported.", source: file:///android_asset/www/index.html (6)
D/CordovaWebViewClient(20207): onPageFinished(file:///android_asset/www/index.html)
D/CordovaActivity(20207): onMessage(onPageFinished,file:///android_asset/www/index.html)
D/Yamaha-MC1N2-Audio( 1849): yamaha_mc1n2_audio_output_stop()
D/Yamaha-MC1N2-Audio( 1849): yamaha_mc1n2_audio_route_start()
D/CordovaActivity(20207): onMessage(spinner,stop)
I/chromium(20207): [INFO:async_pixel_transfer_manager_android.cc(56)] Async pixel transfers not supported
I/chromium(20207): [INFO:async_pixel_transfer_manager_android.cc(56)] Async pixel transfers not supported
D/lights  ( 2263): set_light_buttons: 2
D/lights  ( 2263): set_light_buttons: 1
D/Finsky  (20069): [1] 5.onFinished: Installation state replication succeeded.
D/lights  ( 2263): set_light_buttons: 2
D/lights  ( 2263): set_light_buttons: 1
I/healthd ( 1840): battery l=7 v=3754 t=29.0 h=2 st=2 c=0 chg=u
D/lights  ( 2263): set_light_buttons: 2
D/lights  ( 2263): set_light_buttons: 1
D/lights  ( 2263): set_light_buttons: 2
I/healthd ( 1840): battery l=7 v=3750 t=31.0 h=2 st=2 c=0 chg=u
```
