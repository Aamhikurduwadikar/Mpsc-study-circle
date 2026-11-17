MPSC STUDY CIRCLE – AUTH + CHAT SETUP
=====================================

या ZIP मध्ये:
- Google Login (Firebase Google provider)
- Email/Password Login आणि नवीन Account Registration
- Guest / Anonymous Login बंद
- Real-time Public Chat
- विद्यार्थी यादी आणि Private one-to-one text chat
- MPSC Study Circle – Powered by Majhi_Mpsc branding
- Instagram link: https://www.instagram.com/majhi_mpsc/

Firebase Console मध्ये करावयाच्या आवश्यक सेटिंग्ज:
1) Authentication > Sign-in method मध्ये Google आणि Email/Password Enable करा.
2) Authentication > Settings > Authorized domains मध्ये तुमचा Vercel domain जोडा.
3) Firestore Database > Rules मध्ये firestore.rules मधील नियम Publish करा.
4) Firebase Web App config ही index.html मध्ये आधीपासून आहे; ती तुमच्या Firebase project शी जुळते याची खात्री करा.
5) Email/Password provider वापरताना Email verification सक्तीची करायची असल्यास Firebase Console मधील Email Templates/Authentication settings तपासा.

महत्त्वाचे:
- Google popup साठी Authorized Domains योग्य असणे आवश्यक आहे.
- Firestore Rules publish केल्याशिवाय Chat चालणार नाही.
- Private Chat फक्त त्या room मधील दोन participants साठी आहे.
- ही text-chat आवृत्ती आहे. Image/PDF upload, admin moderation आणि reporting समाविष्ट नाहीत.
- chatUsers मध्ये display name व UID साठवले जातात; संवेदनशील माहिती टाकू नका.
