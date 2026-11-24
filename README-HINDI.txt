AMBITOR ALPHA Android APK Project

यह APK अभी इस प्रोजेक्ट से ऑनलाइन GitHub Actions के जरिए बनवाया जा सकता है।
आपको Android Studio/command line की जरूरत नहीं है, लेकिन GitHub पर प्रोजेक्ट अपलोड करना होगा।

सरल तरीका:
1) GitHub.com पर लॉगिन करें या अकाउंट बनाएं।
2) New repository बनाएं, नाम रखें ambitor-alpha-apk और Public चुनें।
3) Add file > Upload files चुनें।
4) इस ZIP को पहले अपने कंप्यूटर में Extract करें।
5) Extract हुए फोल्डर के अंदर की सभी फाइल/फोल्डर GitHub upload page पर drag-drop करें (फोल्डर के अंदर की चीजें, ZIP नहीं)।
6) Commit changes दबाएं।
7) Repository में Actions टैब खोलें। "Build AMBITOR ALPHA APK" workflow चलेगा।
8) Build पूरा होने पर workflow run खोलें; नीचे Artifacts में AMBITOR-ALPHA-APK डाउनलोड करें।
9) ZIP artifact extract करें; app-debug.apk फोन में भेजकर install करें।

सीमाएं:
- यह debug APK है, Play Store release-signed APK नहीं।
- Work/notes/profile data WebView के local storage में इसी फोन में रहता है; app data clear/uninstall करने से मिट सकता है। JSON backup रखें।
- समय के reminder केवल ऐप खुला रहने पर check होते हैं; ऐप बंद होने पर भरोसेमंद notifications के लिए अलग Android notification scheduling/server push implementation चाहिए।
- APK इस वातावरण में compile/test नहीं किया गया; GitHub Actions compile करेगा। Build failure होने पर error screenshot भेजें।
