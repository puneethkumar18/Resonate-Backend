# Resonate - An Open Source Social Voice Platform

### This project is divided into two repositories:
1. [Resonate Flutter App](https://github.com/AOSSIE-Org/Resonate)
2. Resonate Backend (You are here)

Go to [this repository](https://github.com/AOSSIE-Org/Resonate) to know more about the project.

## Environment Setup :

1. Pre-requisites :

    (a) Clone the Repo : `git clone https://github.com/AOSSIE-Org/Resonate-Backend`

    (b) Run this command to install required dependencies from package.json : `npm install`

2. Create a `.env` file in the project's root directory

3. Follow [this guide](https://docs.livekit.io/cloud/project-management/keys-and-tokens/) to obtain your `HOST`, `API-KEY`, `API-SECRET` from [livekit-cloud](https://livekit.io/cloud).

4. Create a new project on [Appwrite Cloud](https://appwrite.io/) or self host it locally by pulling their [docker image](https://appwrite.io/docs/self-hosting). Know more about Appwrite [here](https://appwrite.io/docs).

5. The `.env` file should consist of :

    (a)`LIVEKIT_API_KEY`

    (b)`LIVEKIT_API_SECRET`

    (c)`LIVEKIT_HOST`

    (d)`LIVEKIT_SOCKET_URL`

    (e)`APPWRITE_ENDPOINT`

    (f)`APPWRITE_PROJECT_ID`

    (g)`APPWRITE_SECRET_API_KEY`

6. There are 3 appwrite cloud functions needed for maintaining the functionality of Resonate

    (a)`send_otp` - Sending emails to users with the otp while email verification

    (b)`verify_otp` - Verifies the user entered otp with the otp sent to his mail for email verification

    (c)`set_email_verified` - Sets the user account as email verified once email verification is successful

    (d)`match_maker` - Used to match requests in pair chat feature

    Each of these functions have their own respective appwrite.json files one for each function which has the API keys used in that function
    and is necessary while using Appwrite's CLI for deployments (commonly preferred).

    The appwrite.json files are put into .gitignore please do request for them on AOSSIE's discord server in order to contribute to Resonate's appwrite cloud functions


## Communication Channels

If you have any questions, need clarifications, or want to discuss ideas, feel free to reach out through the following channels:

-   [Discord Server](https://discord.com/invite/6mFZ2S846n)
-   [Email](mailto:aossie.oss@gmail.com)

We appreciate your contributions and look forward to working with you to make this project even better!
