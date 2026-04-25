# My Academic Pages

- to add section in navigation bar, modify this [file](_data/navigation.yml)
- put pdf files in `files` folder and images in `images` folder

- When modifying `_config.yml`, `_config_docker.yml` or other plugins, run in docker terminal (in VS Code) :
`jekyll serve -H 0.0.0.0 -w --force_polling --config _config.yml,_config_docker.yml`

- to remove the "share on" at the end of page. Set `share` to false in `scope` section in [_config](_config.yml) file.

- to modified the footer of the websites, check out this [file](_includes/footer.html).
- if using Linux, run `systemctl --user start docker-desktop` (start docker desktop application and its associated background services (the Docker engine/daemon) for the current user) before opening Dev Container on VS Code

- to modify basic site settings, links (eg. to social media and so on) check `_config.yml'
- to modify/add pages, see `_pages` folder. For instance, to add info on the about homepage, check out [this file](_pages/about.md)
- for teaching page, see `_teaching` folder



### Using the DevContainer in VS Code

See more info at https://academicpages.github.io/

If you are using [Visual Studio Code](https://code.visualstudio.com/) you can use the [Dev Container](https://code.visualstudio.com/docs/devcontainers/containers) that comes with this Repository. Normally VS Code detects that a development container configuration is available and asks you if you want to use the container. If this doesn't happen you can manually start the container by **F1->DevContainer: Reopen in Container**. This restarts your VS Code in the container and automatically hosts your academic page locally on http://localhost:4000. All changes will be updated live to that page after a few seconds.


## Bugfixes and enhancements

If you have bugfixes and enhancements that you would like to submit as a pull request, you will need to [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) this repository as opposed to using it as a template. This will also allow you to [synchronize your copy](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) of template to your fork as well.

Unfortunately, one logistical issue with a template theme like Academic Pages that makes it a little tricky to get bug fixes and updates to the core theme. If you use this template and customize it, you will probably get merge conflicts if you attempt to synchronize. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch.

---
<div align="center">
    
![pages-build-deployment](https://github.com/academicpages/academicpages.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)
[![GitHub contributors](https://img.shields.io/github/contributors/academicpages/academicpages.github.io.svg)](https://github.com/academicpages/academicpages.github.io/graphs/contributors)
[![GitHub release](https://img.shields.io/github/v/release/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io/releases/latest)
[![GitHub license](https://img.shields.io/github/license/academicpages/academicpages.github.io?color=blue)](https://github.com/academicpages/academicpages.github.io/blob/master/LICENSE)

[![GitHub stars](https://img.shields.io/github/stars/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io)
[![GitHub forks](https://img.shields.io/github/forks/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io/fork)
</div>
