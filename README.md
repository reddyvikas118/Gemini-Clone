# Gemini AI Web App

Gemini AI is an innovative web application that brings an interactive chat experience with the help of Google Gemini Pro api. Built using Node.js, React.js, MongoDB, and Redux Toolkit, this app allows users to engage in text-based conversations with Gemini AI. The application features Google OAuth V2 for user authentication, enabling enhanced capabilities and personalization.

## Description

Gemini AI Web App is a Google Gemini clone, providing users with a seamless chat interface powered by advanced AI capabilities. Users can enjoy conversations with Gemini AI, receiving text-based responses. The application supports two user types:

1. **Non-authenticated Users:**

   - Limited to 10 chat requests per hour.
   - Access to the last 5 chat history entries.

2. **Authenticated Users:**
   - Unlimited chat responses.
   - Full chat history access upon login.
3. **Modern Interface:**
   - Enjoy a clean and user-friendly interface for a seamless chat experience.

## Live Demo

Explore the live demo of Gemini AI: [https://geminichatai.netlify.app/](https://geminichatai.netlify.app/)

![Demo Screenshot](https://res.cloudinary.com/dqone7ala/image/upload/v1710036366/Screenshot_2024-03-10_073520_wkcnwj.png)

## Installation

### Server Side

1. Clone the repository:

   ```bash
   git clone https://github.com/shuvra-matrix/Gemini-Ai--MERN.git
   ```

2. Navigate to the server folder:

   ```bash
   cd ./server
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Set up environment variables in a `.env` file:

   ```
   MONGO_USER=mongodb_username
   MONGO_PASS=mongodb_password
   GEMINI_API_KEY=gemini_api_key
   CLIENT_API_KEY=server_client_verify_api_key(generate by user)
   GEO_API_KEY=ipgeolocation_api_key
   LOCATION_API_KEY=geocode_api_key
   GOOGLE_CLIENT_ID=google_oauth_client_id
   GOOGLE_CLIENT_SECRET=google_oauth_client_secret
   GOOGLE_OAUTH_REDIRECT_URL=google_oauth_redirect_url
   CLIENT_REDIRECT_URL="http://localhost:3000"
   ACCESS_TOKEN_JWT_SECRET=cookie_secret
   REFRESH_TOKEN_JWT_SECRET=cookie_secret
   ACCESS_TOKEN_EXPIRETIME=15m
   REFRESH_TOKEN_EXPIRETIME=7d
   APPLICATION_TYPE="dev" or"production"
   COOKIE_DOMAIN=serverid_domain
   ```

5. Run the server:

   ```bash
   npm start
   ```

### Client Side

1. Navigate to the root directory:

   ```bash
   cd Gemini-Ai--MERN
   ```

2. Install client dependencies:

   ```bash
   npm install
   ```

3. Set up client-side environment variables in a `.env` file:

   ```
   REACT_APP_GEMINI_KEY=user_generated_key)
   REACT_APP_GOOGLE_CLIENT_ID=google_oauth_client_id
   REACT_APP_GOOGLE_CLIENT_SECRET=google_oauth_client_secret
   REACT_APP_GOOGLE_OAUTH_REDIRECT_URL=google_oauth_redirect_url
   REACT_APP_SERVER_ENDPOINT=http://localhost:3030
   ```

4. Run the client:

   ```bash
   npm start
   ```

## Docker Setup

If you have Docker installed, use the following command in the root directory:

```bash
docker-compose -f docker-compose.yaml up
```

## Location Tracking

Gemini AI Web App employs location tracking features for enhanced user experience. The following APIs are utilized on the server side to obtain location and IP details:

1. **IP Geolocation API:**

   - Used to retrieve initial location details based on the user's IP address.
   - API Endpoint: [https://ipgeolocation.io/](https://ipgeolocation.io/)
   - This information helps in providing a general idea of the user's location.

2. **Geocode API:**
   - Utilized to get precise user location details by updating location based on latitude and longitude.
   - API Endpoint: [https://geocode.maps.co/](https://geocode.maps.co/)
   - The app uses this API to convert latitude and longitude coordinates into an accurate user location.

If you have any concerns or questions regarding the use of location tracking in Gemini AI Web App, please contact us at [reddyvikas1618@gmail.com](reddyvikas1618@gmail.com).
Enjoy chatting with Gemini AI! 🚀
