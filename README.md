# ReVanced Modules

[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/elohim_etz)
[![CI](https://github.com/j-hc/revanced-magisk-module/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/elohim-etz/revanced-modules/actions/workflows/ci.yml)

Extensive ReVanced builder

Get the [latest CI release](https://github.com/elohim-etz/revanced-modules/releases).

Use [**zygisk-detach**](https://github.com/j-hc/zygisk-detach) to detach YouTube and YT Music from Play Store if you are using modules.

<details><summary><big>Features</big></summary>
<ul>
 <li>Support all present and future ReVanced and <a href="https://github.com/anddea/revanced-patches">ReVanced Extended</a> apps</li>
 <li> Can build Magisk/KernelSU modules and non-root APKs</li>
 <li> Updated daily with the latest versions of apps and patches</li>
 <li> Optimize APKs and modules for size</li>
 <li> Modules</li>
    <ul>
     <li> recompile invalidated odex for faster usage</li>
     <li> receive updates from Magisk/KernelSU app</li>
     <li> do not break safetynet or trigger root detections</li>
     <li> handle installation of the correct version of the stock app and all that</li>
     <li> support Magisk and KernelSU</li>
    </ul>
</ul>
Note that the <a href="../../actions/workflows/ci.yml">CI workflow</a> is scheduled to build the modules and APKs everyday using GitHub Actions if there is a change in ReVanced patches. You may want to disable it.
</details>

## To include/exclude patches or patch other apps

- Star the repo :eyes:
- Use the repo as a [template](https://github.com/new?template_name=revanced-modules&template_owner=elohim-etz)
- Customize [`config.toml`](./config.toml) using [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
- Run the build [workflow](../../actions/workflows/build.yml)
- Grab your modules and APKs from [releases](../../releases)

also see here [`CONFIG.md`](./CONFIG.md)

## Building Locally

### On Termux

```console
bash <(curl -sSf https://raw.githubusercontent.com/elohim-etz/revanced-modules/main/build-termux.sh)
```

### On Desktop

```console
$ git clone https://github.com/elohim-etz/revanced-modules
$ cd revanced-modules
$ ./build.sh
```
