# All Print Admin Panel — GitHub Pages

यह फ़ोल्डर GitHub Pages पर Admin Panel होस्ट करने के लिए है।

## फ़ाइलें
- `index.html` — Admin Panel की मुख्य HTML फ़ाइल।
- `README.md` — GitHub पर अपलोड और Pages सेटअप करने के निर्देश।

## GitHub पर चलाने का तरीका
1. GitHub में नया repository बनाएँ, उदाहरण: `All-Print-Admin`.
2. इस फ़ोल्डर की दोनों फ़ाइलें (`index.html` और `README.md`) repository के मुख्य स्तर (root) पर अपलोड करें। ZIP फ़ाइल को सीधे repository में डालने के बजाय पहले ZIP खोलें और अंदर की फ़ाइलें अपलोड करें।
3. Repository में **Settings → Pages** खोलें।
4. **Build and deployment** में Source को **Deploy from a branch** चुनें।
5. Branch `main` और folder `/(root)` चुनकर **Save** दबाएँ।
6. Deployment पूरा होने के बाद लिंक होगा: `https://YOUR-GITHUB-USERNAME.github.io/All-Print-Admin/`

## ध्यान दें
- अगर repository का नाम या GitHub username अलग है, तो लिंक उसी के अनुसार बदल जाएगा।
- पहली बार प्रकाशित होने में कुछ मिनट लग सकते हैं।
- `README.md` निर्देशों के लिए है; Admin Panel चलाने के लिए `index.html` आवश्यक है।
- केवल GitHub पर होस्ट करने से Firebase/Firestore अपने-आप कनेक्ट नहीं होता। Shared data के लिए Firebase configuration और सुरक्षित Firestore Rules अलग से सही होने चाहिए।
- Admin पेज का URL छिपाना सुरक्षा नहीं है। Firestore में write access केवल Owner UID को दें। कभी भी सार्वजनिक read/write नियम (`allow read, write: if true`) न लगाएँ।
