# Pushwoosh Unity SDK

[![GitHub release](https://img.shields.io/github/release/akidison/pushwoosh-unity.svg?style=flat-square)](https://github.com/akidison/pushwoosh-unity/releases)
![platforms](https://img.shields.io/badge/platforms-Android%20%7C%20iOS%20%7C%20Windows-yellowgreen.svg)

Push notification SDK for Unity. Wraps native Pushwoosh iOS and Android SDKs.

## Installation

### Option 1: UPM via Git URL (recommended)

In Unity: **Window > Package Manager > + > Add package from git URL**

Add core package first, then platform packages you need:

```
https://github.com/akidison/pushwoosh-unity.git?path=com.akidislab.unity.pushwoosh.core
https://github.com/akidison/pushwoosh-unity.git?path=com.akidislab.unity.pushwoosh.android
https://github.com/akidison/pushwoosh-unity.git?path=com.akidislab.unity.pushwoosh.ios
https://github.com/akidison/pushwoosh-unity.git?path=com.akidislab.unity.pushwoosh.windows
```

To pin a specific version, add `#X.Y.Z`:

```
https://github.com/akidison/pushwoosh-unity.git?path=com.akidislab.unity.pushwoosh.core#1.0.7
```

### Option 2: .unitypackage

Download `Pushwoosh.unitypackage` from [Releases](https://github.com/akidison/pushwoosh-unity/releases) and import via **Assets > Import Package > Custom Package**.

For iOS Notification Service Extension, also import `AddNotificationServiceExtensioniOS.unitypackage`.

## Requirements

- Unity 2020.3+
- **Android**: [External Dependency Manager for Unity (EDM4U)](https://github.com/googlesamples/unity-jar-resolver) is required to resolve native dependencies
- **iOS**: CocoaPods (auto-configured by the SDK, or via EDM4U)
- **Windows**: No additional dependencies required

## Quick Start

```csharp
using UnityEngine;

public class PushwooshExample : MonoBehaviour
{
    void Start()
    {
        Pushwoosh.ApplicationCode = "XXXXX-XXXXX";
        Pushwoosh.FcmProjectNumber = "YOUR_FCM_NUMBER";

        Pushwoosh.Instance.OnRegisteredForPushNotifications += (token) => {
            Debug.Log("Push token: " + token);
        };

        Pushwoosh.Instance.OnPushNotificationsReceived += (payload) => {
            Debug.Log("Push received: " + payload);
        };

        Pushwoosh.Instance.RegisterForPushNotifications();
    }
}
```

## Documentation

https://www.pushwoosh.com/platform-docs/pushwoosh-sdk/cross-platform-frameworks/unity

## License

Pushwoosh Unity SDK is released under the MIT license.
