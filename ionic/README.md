# Ionic

Just a repo that stores frequently used commands from ionic

## 🚧 Development

#### Install Ionic CLI globally

This command will install Ionic CLI in your devices so that you can execute commands in terminal.

```
npm install -g @ionic/cli
```

#### View commands

This command will list out all commands that you can used with Ionic CLI.

```
ionic --help
```

#### Start ionic in web

This command will run Ionic project in web browser.

```
ionic serve
```

#### Start ionic in app

This command will run Ionic project in android emulator (**--external**) with live reload (**-l**).

```
ionic cap run android -l --external
```

#### Build Ionic

This command will generate a build folder from your Ionic project.

```
ionic build
```

#### Copy

This command will copy codes from web to native platform (IOS/Android)

```
ionic cap copy
```

#### Sync

This command will synchronise the installed plugins from capacitor with the native platforms (IOS/Android). This command will copy codes from web to native platform (IOS/Android)

```
ionic cap sync
```

## 📦 Capacitor Plugins

#### Install plugin

You may find available plugins from [capacitor](https://capacitorjs.com/docs/plugins) website.

```
npm install @capacitor/<<plugin_name>>
```

#### Uninstall plugin

```
npm uninstall @capacitor/<<plugin_name>>
```

#### Sync

For detailed explanation, view [this](#sync).

```
ionic cap sync
```
