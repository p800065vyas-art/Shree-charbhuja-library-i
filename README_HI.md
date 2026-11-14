# Shree Charbhuja Library Android App — v1.1

यह Android Studio के लिए starter source project है, पहले चरण में निम्न काम करता है:
- 60 साझा सीटों में सीट 1–60 आवंटन; एक सीट पर एक सक्रिय विद्यार्थी
- Full Day / Morning / Evening शिफ्ट दर्ज करना
- विद्यार्थी रजिस्टर और सूची
- फीस रिकॉर्ड (डिफॉल्ट ₹600; भुगतान राशि संपादन योग्य)
- रोज़ की हाजिरी (हाजिर / गैरहाजिर)
- कुल विद्यार्थी और कुल जमा फीस रिपोर्ट
- SQLite लोकल डेटाबेस

## Build
1. ZIP extract करें और Android Studio में फ़ोल्डर खोलें।
2. Android Studio में Gradle Sync करें (JDK 17, Android SDK 35)।
3. Android फोन USB debugging से जोड़ें और Run दबाएँ।
4. APK बनाने के लिए Build > Build Bundle(s) / APK(s) > Build APK(s) चुनें।

## महत्वपूर्ण सीमाएँ
- यह source project है, पहले से compiled APK नहीं।
- लोकल डेटा ऐप के private storage में रहता है। ऐप uninstall, फोन खराब या reset होने पर डेटा खो सकता है।
- इस संस्करण में export/restore backup, admin PIN, फीस बकाया गणना, छात्र संपादन/डिलीट, attendance history और PDF रसीद अभी शामिल नहीं हैं। वास्तविक उपयोग से पहले इन सुविधाओं को जोड़ना और डेटा बैकअप टेस्ट करना चाहिए।
- सीटें shared pool हैं: एक सीट नंबर किसी भी शिफ्ट में एक ही सक्रिय विद्यार्थी को दिया जा सकता है। यदि एक ही भौतिक सीट को अलग-अलग शिफ्ट में अलग विद्यार्थियों को देना हो तो seat/shift allocation नियम बदलना होगा।
