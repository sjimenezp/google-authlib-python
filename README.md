## Example Code: Using OAuth2/OpenID Connect Authentication with Authlib, Flask, and Google

This is an example code repository demonstrating how to implement OAuth2/OpenID Connect authentication with Google using the Authlib library and Flask framework. OAuth2/OpenID Connect is a widely used authentication framework that allows users to authenticate with third-party providers such as Google.

### Configuration

To use OAuth2/OpenID Connect authentication with Google, you need to obtain Google API credentials. Follow these steps to set up your credentials:

-Go to the Google Cloud Console.
-Create a new project or select an existing one.
-Enable the Google+ API in the APIs & Services > Library section.
-Go to APIs & Services > Credentials and click on Create Credentials.
-Choose OAuth client ID as the credential type.
-Select Web application as the application type.
-Enter a name for your OAuth client ID (e.g., "Flask Auth App").
-Add http://localhost:5000/auth as an Authorized redirect URI.
-Click Create to create the OAuth client ID.
-Copy the Client ID and Client Secret values.
-Open the config.py file in the code repository and replace the placeholders with your actual credentials (or with environment variables):

```python
# config.py

GOOGLE_CLIENT_ID = 'your_client_id'
GOOGLE_CLIENT_ID = 'your_client_secret'
```
