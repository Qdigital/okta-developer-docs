---
title: Handle the Callback from Okta
---

After Okta authenticates a user, they're redirected back to your application via the callback route you [defined earlier]. When Okta redirects back, the URL fragment (the portion after `#`) will contain either tokens for the user, or an error if something went wrong.

Your application must parse this information, and if tokens are present, store the user's tokens.

<StackSelector snippet="handle-callback"/>

<button>I've wired up the callback route</button>