This is a fork of cordova-plugin-firebasex. You can read the original documentation here: https://github.com/dpa99c/cordova-plugin-firebasex.git

### Modifications:
Added a new branch called `v17-fixed` that serves two purposes:

1. In v18.0.0 changes happened to the notifications mechanism and onMessageReceived wouldn't get triggered after cold start. I've opened this issue in the original repo: https://github.com/dpa99c/cordova-plugin-firebasex/issues/917
2. Added access to FIRAuthErrorUserInfoUpdatedCredentialKey on linkUserWithCredential auth/credential-already-in-use error. I've opened this pull request in the original repo: https://github.com/dpa99c/cordova-plugin-firebasex/pull/916. It has been accepted and merged to v18.0.5 but we can't use this version because the notifications problem.
