## AppPredictionInternal

> `/System/Library/PrivateFrameworks/AppPredictionInternal.framework/AppPredictionInternal`

```diff

-468.23.0.0.0
-  __TEXT.__text: 0x4214f4
+468.23.1.0.0
+  __TEXT.__text: 0x4216bc
   __TEXT.__stubs: 0x1350
-  __TEXT.__objc_methlist: 0x319d0
+  __TEXT.__objc_methlist: 0x319e0
   __TEXT.__const: 0x387c
   __TEXT.__cstring: 0x4a620
-  __TEXT.__oslogstring: 0x2e1a4
+  __TEXT.__oslogstring: 0x2e210
   __TEXT.__gcc_except_tab: 0xe868
   __TEXT.__ustring: 0x4
-  __TEXT.__unwind_info: 0xbb34
+  __TEXT.__unwind_info: 0xbb38
   __TEXT.__eh_frame: 0x12c
   __TEXT.__objc_classname: 0x74a8
-  __TEXT.__objc_methname: 0x9ae42
+  __TEXT.__objc_methname: 0x9ae69
   __TEXT.__objc_methtype: 0x1737a
-  __DATA_CONST.__got: 0x1418
+  __DATA_CONST.__got: 0x1420
   __DATA_CONST.__const: 0xdab0
   __DATA_CONST.__cfstring: 0x360a0
   __DATA_CONST.__objc_classlist: 0x1988

   __DATA_CONST.__objc_protolist: 0x360
   __DATA_CONST.__objc_imageinfo: 0x8
   __DATA_CONST.__objc_const: 0x708d8
-  __DATA.__objc_selrefs: 0x19b08
+  __DATA.__objc_selrefs: 0x19b10
   __DATA.__objc_protorefs: 0x30
   __DATA.__objc_classrefs: 0x2488
   __DATA.__objc_superrefs: 0x1310

   - /usr/lib/libcompression.dylib
   - /usr/lib/libobjc.A.dylib
   - /usr/lib/libsqlite3.dylib
-  Functions: 21537
-  Symbols:   31813
-  CStrings:  29781
+  Functions: 21538
+  Symbols:   31815
+  CStrings:  29783
 
Symbols:
+ -[ATXNotificationAndSuggestionDatabase _purgeNotificationBiomeStreamsIfNeeded]
+ __kATXBiomeNotificationPurgeCompleteKey
Functions:
~ -[ATXNotificationAndSuggestionDatabase init] : 60 -> 96
+ -[ATXNotificationAndSuggestionDatabase _purgeNotificationBiomeStreamsIfNeeded]
~ -[ATXNotificationsLoggingServer logNotificationEvent:notification:reason:] : 1352 -> 1448
CStrings:
+ "ATXNotificationAndSuggestionDatabase: Purging private notification streams to remove persisted text content"
+ "_purgeNotificationBiomeStreamsIfNeeded"
```
