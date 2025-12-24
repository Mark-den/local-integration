# Account Access System (Facebook Login)

A secure authentication system that allows users to log in using their Facebook account and view their profile information.

## Features

- **Facebook OAuth Authentication**: Secure login using Facebook credentials
- **Profile Display**: Shows user's name, email, and profile picture after login
- **Logout Functionality**: Secure logout with session clearing
- **Modern UI**: Clean and professional authentication interface
- **Responsive Design**: Works seamlessly across different device sizes

# Facebook Login — Demo

This repository contains a small frontend demo that shows how to integrate the Facebook JavaScript SDK to sign in users and display basic profile information. It is an educational example — not production-ready.

## Features

- Login with Facebook (Facebook JavaScript SDK)
- Display user name, email (if permitted) and profile picture
- Logout and session clearing
- Simple, responsive UI

## Quickstart

1. Clone or download the repository.
2. Serve the folder (recommended) or open `index.html` in a browser. Serving via HTTP/HTTPS is recommended because some browsers restrict SDK behavior on `file://`.

Recommended quick servers:

```powershell
python -m http.server 8000
# or (Node.js)
npx http-server -p 8000
```

Then open `http://localhost:8000` in your browser.

## Configuration

1. Create a Facebook App at https://developers.facebook.com and note the App ID.
2. Update the `appId` value in `script.js` to your App ID.
3. Make sure your app's settings include the correct OAuth redirect URIs / valid origins for local testing (e.g. `http://localhost:8000`).

Important: never include your App Secret in client-side code. This demo only requires the public App ID.

## Files

- index.html — demo UI and SDK loader
- script.js — Facebook SDK init, login/logout and profile handling
- style.css — styles for the demo

## Notes

- This project is a frontend demo. For a secure production implementation you must validate tokens server-side and follow Facebook's best practices.
- Permissions requested in the demo are limited to `public_profile` and `email`.

## Where to look next

- Edit `script.js` to set your Facebook App ID and adjust requested permissions.
- Run the local server and test the login flow in the browser.

---



