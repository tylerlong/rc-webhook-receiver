# RingCentral WebHook Receiver

This is a server side application to receive RingCentral WebHook notifications.

Please note that: it's for **testing** only, not for production, since there is no security built-in.

# Deploy to render.com (free)

Click the button below to deploy this application to Render:

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

## Important URLs

You will be able to find the public URL of your deployed web serice on the top left of the page. It is of format `https://<name-of-your-deployment>.onrender.com`.

The URL for webhook is: `https://<name-of-your-deployment>.onrender.com/webhook/`

The URL to view received notifications is `https://<name-of-your-deployment>.onrender.com/read/`

## Create WebHook

https://developers.ringcentral.com/api-reference/Subscriptions/createSubscription

Don't forget to use `https://<name-of-your-deployment>.onrender.com/webhook/` as WebHook URL.

## Check notifications

Go to `https://<name-of-your-deployment>.onrender.com/read/`.

Please note that, only the latest 100 notifications are shown.

The notifiations are saved in memory, so if you restart your server or redeploy the service, the notifications may disappear. I said at the beginning, this project is for testing only.

## Limitations

> Your free instance will spin down with inactivity, which can delay requests by 50 seconds or more.

So before you test, you need to access `https://<name-of-your-deployment>.onrender.com/read/` to activate your app.

# Deploy to heroku.com (paid hosting)

Click the button below to deploy this application to Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/tylerlong/rc-webhook-receiver)

Other instructions are similar to render.com instructions. Just replace `https://<name-of-your-deployment>.onrender.com` with your heroku app's URL.
