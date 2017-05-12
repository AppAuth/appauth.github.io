
AppAuth is a client SDK for native apps to authenticate and authorize end-users
using [OAuth 2.0](https://tools.ietf.org/html/rfc6749) and [OpenID Connect](http://openid.net/specs/openid-connect-core-1_0.html). Available for [iOS](https://github.com/openid/AppAuth-iOS),
[macOS](https://github.com/openid/AppAuth-iOS), [Android](https://github.com/openid/AppAuth-Android) and 
[Native JS](https://github.com/openid/AppAuth-JS) environments, it implements modern security and usability
[best practices](https://tools.ietf.org/html/draft-ietf-oauth-native-apps) for
native app authentication and authorization.

It strives to directly map the requests and responses of those specifications, while following
the idiomatic style of the implementation language. In addition to mapping the
raw protocol flows, convenience methods are available to assist with common
tasks like performing an action with fresh tokens.

It follows the best practices set out in 
[OAuth 2.0 for Native Apps](https://tools.ietf.org/html/draft-ietf-oauth-native-apps)
including using in-app browser tabs (i.e. SFSafariViewController or Android Custom Tabs)
where available. For this reason, embedded user-agents (known as web-views) are explicitly
*not* supported due to usability and security reasons.

It also supports the [PKCE](https://tools.ietf.org/html/rfc7636) extension to
OAuth which was created to secure authorization codes in public clients when
custom URI scheme redirects are used. The library is friendly to other
extensions (standard or otherwise) with the ability to handle additional params
in all protocol requests and responses.
