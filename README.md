# PhoneRemote (starter project)

This Android project builds two APK variants with GitHub Actions:
- Controller: installed on the controller phone.
- Receiver: installed on the phone whose owner has agreed to use it.

## Important current limitation
This is a **starter build**, not yet an internet-connected remote-control system. The controller APK currently displays setup information. The receiver APK can request Android's visible Device Admin permission and perform a local screen-lock test after the phone's user explicitly enables it.

There is no hidden control, forced shutdown, remote lock, or background command receiver in this starter. Internet pairing and command delivery require a backend and must be added and tested in a later step.

## Build
Push this project to a GitHub repository. Open **Actions** → **Build PhoneRemote APKs** → **Run workflow**. Download the `PhoneRemote-APKs` artifact from the successful run.

## Test safely
Install the receiver APK on the receiver phone. Open it and review the explanation before enabling screen-lock permission. Try the local lock test only when the phone's owner agrees and knows the screen will lock.
