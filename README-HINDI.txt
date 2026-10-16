ALL PRINT ADMIN PANEL — GITHUB PAGES

1) GitHub par naya repository banayein: All-Print-Admin
2) Repository Public rakhein (GitHub Free Pages ke liye).
3) Is folder ke andar ki index.html aur firestore.rules.txt ko repository ke root mein upload karein.
4) Settings > Pages > Build and deployment mein:
   Source: Deploy from a branch
   Branch: main
   Folder: / (root)
   Save karein.
5) Actions/Pages deployment successful hone ke baad link:
   https://chandramohan2026.github.io/All-Print-Admin/

IMPORTANT:
- Admin panel ko alag repository mein rakhein. Main All-Card-Print repository ki index.html ko replace na karein.
- Firebase Console > Authentication mein Email/Password enabled hona chahiye.
- Firestore Rules ko check karke hi publish karein. Public config read allowed aur write sirf owner UID ke liye hona chahiye.
- GitHub Pages par rakhi HTML public source hoti hai; password/API config ko secret na samjhein. Owner security Firebase Authentication + Firestore Rules se enforce honi chahiye.
- Agar site 404 de, Settings > Pages par publishing source aur latest deployment check karein; GitHub Pages ko deploy hone mein kuch minutes lag sakte hain.
