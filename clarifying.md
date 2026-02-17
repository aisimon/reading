feature vs. reality


Option 1: Direct & Investigative
Tone: Professional and efficient.
@developers 👀 I am verifying my understanding of the login process for The Integrated Portal, would appreciate a quick sanity check: 👀
From what I can see, our The Core Platform users access The Integrated Portal by clicking a "Login" link inside the main dashboard. The Core Platform then logs them in automatically. At no point are they required to manually enter credentials, which means there’s no practical need for them to change a password.
The account used is a system-level user, and it seems the flow was never designed for manual credential entry.
The reason I ask is that I have a case where a user changed their password inside The Integrated Portal's dashboard and is now blocked out. Does this align with how the integration is supposed to work?

Option 2: The Logic Verification
Tone: Collaborative and focused on the technical "why."
Hey @developers, quick question on the The Core Platform -> The Integrated Portal handshake. 🤝
Am I right in thinking that these accounts are strictly SSO-only? My understanding is that the system handles authentication entirely in the background, so the user never actually "owns" a password they would need to type in manually.
I’m asking because a user managed to trigger a password change within the The Integrated Portal settings and is now unable to get back in. If manual logins aren't supported for these integrated accounts, did this change break the automated link?

Option 3: Short & Punchy
Tone: Casual and direct.
@developers 💡 Quick Sanity Check:
Are The Integrated Portal users meant to be SSO-only when coming from The Core Platform?
I was under the impression they never use manual credentials because the system logs them in automatically. I’ve got a user who manually changed their password in the portal dashboard and is now locked out.
If manual logins aren't part of the design, should that "Change Password" option even be visible to this type of user?


