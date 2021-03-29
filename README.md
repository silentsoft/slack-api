# Slack API

![release](https://img.shields.io/badge/release-0.1.1-blue.svg)
[![Build Status](https://travis-ci.com/silentsoft/slack-api.svg?branch=master)](https://travis-ci.com/silentsoft/slack-api)
[![license](https://img.shields.io/badge/license-Apache--2.0-green.svg)](https://github.com/silentsoft/slack-api/blob/master/LICENSE.txt)
[![HitCount](http://hits.dwyl.com/silentsoft/slack-api.svg)](http://hits.dwyl.com/silentsoft/slack-api)

`Slack API` is a simple Java library to post a Slack message to specific channel.

## Features
  - [postMessage](https://api.slack.com/methods/chat.postMessage)
    - ```java
      SlackAPI.postMessage("xxxx-xxxxxxxxx-xxxx", "general", "Hello, World !");
      ```

## Creating Token
  - token can be generated by two ways.

    - [legacy-tokens](https://api.slack.com/custom-integrations/legacy-tokens)
      1. Visit Legacy Tokens page at https://api.slack.com/custom-integrations/legacy-tokens.
      2. Click Create token.

    - [apps](https://api.slack.com/apps)
      1. Create an App from https://api.slack.com/apps.
      2. Features > OAuth & Permissions > Scopes > Bot Token Scopes > "channels:read", "chat:write".
      3. Features > OAuth & Permissions > OAuth Tokens & Redirect URLs > Install App to Workspace.
      4. Add an App to specific channel.

## Dependency
```
<dependencies>
    <dependency>
        <groupId>org.silentsoft</groupId>
        <artifactId>slack-api</artifactId>
        <version>0.1.1</version>
    </dependency>
</dependencies>
``` 

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please note we have a [CODE_OF_CONDUCT](https://github.com/silentsoft/slack-api/blob/master/CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.

## License
Please refer to [LICENSE](https://github.com/silentsoft/slack-api/blob/master/LICENSE.txt) and [NOTICE](https://github.com/silentsoft/slack-api/blob/master/NOTICE.md).
