# Langur AI — ওয়েবসাইট হিসেবে প্রকাশ

এই প্রজেক্টে `index.html` হলো ওয়েব UI এবং `server.js` হলো Gemini API-র Backend।

## অনলাইনে প্রকাশ করার ধাপ

1. এই ফোল্ডারের ফাইলগুলো GitHub repository-তে আপলোড করো। `.env` বা API Key কখনো আপলোড করবে না।
2. Render বা Railway-তে Node web service হিসেবে deploy করো।
3. Install command: `npm install`
4. Start command: `npm start`
5. Hosting dashboard-এর Environment Variables-এ যোগ করো:
   - `GEMINI_API_KEY` = Google AI Studio থেকে তৈরি করা নতুন API key
   - `GEMINI_MODEL` = `gemini-2.5-flash`
6. Deploy শেষে hosting provider একটি URL দেবে। সেটি খুললেই Langur AI ওয়েবসাইট ব্যবহার করতে পারবি।

Frontend ও backend একই Node service-এ রাখা হয়েছে; তাই আলাদা API URL সেট করার দরকার নেই।

## গুরুত্বপূর্ণ
- আগে প্রকাশ করা API Key revoke করে নতুন Key ব্যবহার করো।
- API quota বা billing সীমা থাকতে পারে।
- চ্যাট হিস্ট্রি ও শেখানো নোট বর্তমানে ওই browser-এর localStorage-এ থাকে; অন্য ডিভাইসে স্বয়ংক্রিয়ভাবে sync হয় না।
- ফাইলগুলো ওয়েব ডেপ্লয়ের জন্য প্রস্তুত, কিন্তু কোনো hosting account-এ এখনও deploy করা হয়নি।
