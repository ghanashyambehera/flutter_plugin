# flutter_plugin

Parent repository for reusable Flutter modules. Each module is a **git submodule** with its own GitHub repo.

## Modules

| Submodule | Repository | Kind |
|-----------|------------|------|
| `flutter_mobile_diagnostics` | [ghanashyambehera/flutter_mobile_diagnostics](https://github.com/ghanashyambehera/flutter_mobile_diagnostics) | Flutter plugin (Android / iOS) |
| `flutter_network_core` | [ghanashyambehera/flutter_network_core](https://github.com/ghanashyambehera/flutter_network_core) | Dart package (Dio network layer) |

## Clone

```bash
git clone --recurse-submodules https://github.com/ghanashyambehera/flutter_plugin.git
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Update a module

Work inside the submodule, commit, and push that repo. Then in this parent repo:

```bash
cd flutter_network_core
git pull origin main
cd ..
git add flutter_network_core
git commit -m "Bump flutter_network_core"
git push
```
