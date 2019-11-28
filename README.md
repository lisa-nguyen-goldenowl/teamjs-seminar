# Teamjs-seminar notes:

## Alan (7/11/2019)
#### oh-my-zsh: framework to configure terminal
- https://github.com/robbyrussell/oh-my-zsh
#### Reactotron: debug tool for react-native and react (especially for react-native)
- https://github.com/infinitered/reactotron
#### babel-plugin-modules-resolver: sort import 
- https://github.com/tleunen/babel-plugin-module-resolver
- Eslint plugin
- Visual Code plugin
#### webpack-bundle-analyser: Visualize size of webpack output files with an interactive zoomable treemap.
- https://github.com/webpack-contrib/webpack-bundle-analyzer
#### ngrok: exposes local servers to the public internet.
- https://ngrok.com/download

## Nolan (21/11/2019)
#### FlowJS: library support type checking for data flow similar to TypeScript
- Homepage: https://flow.org/en/docs/getting-started/
- Plugin for ESLint to remove warnings when integrating flow: https://github.com/gajus/eslint-plugin-flowtype
#### PostCSS: preprocessor for CSS that supports plugins
- Homepage: https://postcss.org/
- Brief guide:
    - https://blog.logrocket.com/getting-started-with-postcss-in-2019-484262a4d725/
    - https://dev.to/puritanic/add-postcss-to-create-react-app--5hj8
- Common plugins:
    - [Autoprefixer](https://github.com/postcss/autoprefixer)
    - [Nested rule](https://github.com/postcss/postcss-nested)
## Lisa (26/11/2019)
#### Fastlane - the easiest way to automate beta deployments and releases for your iOS and Android apps.
- Homepage: https://docs.fastlane.tools/
- Artical: https://carloscuesta.me/blog/shipping-react-native-apps-with-fastlane/
- install:
    ``` 
    # Using RubyGems

    sudo gem install fastlane -NV

    # Alternatively using Homebrew

    brew cask install fastlane
    ```
    Navigate to your iOS or Android app and run

    ```
    fastlane init
    ```
#### CodePush - a cloud service from Microsoft that gives us the ability to instantly push updates to a react-native application
- Home page: https://github.com/microsoft/react-native-code-push
- Artical: https://carloscuesta.me/blog/react-native-meets-codepush/
- install codepush:
    ```
    $ npm i -g code-push-cli
    $ code-push register
    ```
- Add react-native-code-push as a dependency 
    ```
    $ yarn add react-native-code-push
    $ react-native link react-native-code-push
    ```
    _Note:no need link in version >0.60 react-native_ 

- Release and deploy
    ```
    # code-push release-react <appName> <platform> [options]
    $ code-push release-react codePushRN-ios ios -d Production
    ```
