# About Extole’s SDK and Why You Should Use It
Extole’s Mobile SDK for iOS / Android allow you to load content through native build code or launch a WebView hosted experience in-app.

The Extole SDK allows you to easily:

Initialize a connection from your Mobile App to your Extole marketing programs

Identify your users to Extole to power capabilities for targeting campaigns, delivering appropriate rewards, executing A/B tests, and more. Identification also allows for consistent consumer experiences across your mobile app and other environments.

Load Content from Extole for the appropriate campaign, which is useful for calls-to-action or if you are building in-app experiences that don’t use Extole’s preconfigured content elements.

Launch a WebView sharing experience for the Extole-hosted campaign.

iOS repository: [GitHub](https://github.com/extole/ios)

Android repository: [GitHub](https://github.com/extole/android)

# Getting Started
Understanding Programs, Campaigns, and Zones
The Extole SDK/API functions by interaction with Programs, Campaigns, and Zones inside of your marketing program.

Program
A high-level marketing program you’ve targeted to a specific audience.  A program could be your “refer-a-friend” program or “influencer” program or a “welcome offer” program.

Campaign
Inside of a Program, there may be multiple campaigns. In general, as a developer, you do not need to understand what campaigns are active. When requesting content for a specific program, the Extole targeting engine will determine the appropriate campaign to return. For example, if you request content for your refer-a-friend program and the program is running an A/B test, Extole will determine whether to provide the A Variant Campaign or B Variant Campaign. This happens seamlessly in the SDK and underlying API.

Zone
A zone is a specific piece of content inside of a campaign.  For example, you may have a “mobile_menu” zone, that would provide the icon and text to render in the mobile menu. You may have a “homepage_tile” zone that would tell you the proper image to render on the homepage. The content of the zones is controlled by the marketing team through the My Extole admin app, allowing marketers to dynamically control the content and make sure it's consistent across mobile app, mobile web, desktop web, etc.

## Dependencies

### Repository
```
maven {
    name "github"
    url "https://maven.pkg.github.com/extole/android-sdk"
}
```

### Gradle Dependency
```
implementation 'com.extole.mobile:android-sdk:1.0.+'
```

## 0 Code initializing

{{< gist daniftodi 5914087dca824853a398a8a66b6e4c3a >}}

### SDK APIs Documentation

<iframe width='100%' height='800px' frameborder='none' src="/mobile/android/index.html"></iframe>