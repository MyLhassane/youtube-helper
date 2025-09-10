YouTube Helper
🎯 Goal

The original idea of this project was very simple:
To display and read aloud on a phone the information of the YouTube video currently being watched on a TV or any other device.
This was meant to help people who cannot easily read the video title, description, or even comments.

⚙️ What works

✅ Login with Google account using OAuth2.

✅ Fetching some data from YouTube API (e.g., last uploaded video, public activities).

✅ Text-to-Speech integration to read title and description aloud.

🚧 What does not work

❌ Access to Watch History:

The YouTube Data API does not allow access to the user’s watch history.

Even with full user consent and proper OAuth authentication, the watch history remains restricted.

As a result, the app cannot automatically detect the currently watched video.

😕 Current Status

After multiple iterations and attempts, the project hit a hard limitation: Google’s API restrictions block the very core of the idea.
This leaves the project incomplete and unable to deliver on its main purpose.

📌 Notes

The code may still serve as a reference for learning how to use Google OAuth2 with the YouTube API.

It can also be useful for other allowed use-cases (channel uploads, activities, video metadata, etc.).

But it will not provide watch history access, which was the heart of this project.

📝 Conclusion

This project is a practical example that shows an important reality:
👉 Not everything you can access in YouTube’s web interface as a user is available through the official API.
This contradiction is frustrating, but it demonstrates the limitations faced by independent developers when running into corporate restrictions.