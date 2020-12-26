# jekyll-rtd-theme тема

![CI](https://github.com/rundocs/jekyll-rtd-theme/workflows/CI/badge.svg?branch=develop)
![jsDelivr](https://data.jsdelivr.com/v1/package/gh/rundocs/jekyll-rtd-theme/badge)

Just another documentation theme compatible with GitHub Pages

## What it does?

This theme is inspired by [sphinx-rtd-theme](https://github.com/readthedocs/sphinx_rtd_theme) and refactored with:

- [@primer/css](https://github.com/primer/css)
- [github-pages](https://github.com/github/pages-gem) ([dependency versions](https://pages.github.com/versions/))

``` bash
# Создание пустого удалённого репозитория на github
# Клонирование удалённого репозитория в рабочий клиент
# В тестовом репозитории нужно скопировать хук для UTF-8 и отключить подпись
git config commit.gpgsign false
```

## Quick start

```yml
remote_theme: rundocs/jekyll-rtd-theme
```

{% include list.liquid all=false %}


{% raw %}{{ site.baseurl }}/{{ page.path }}{% endraw %} `{{ site.baseurl }}/{{ page.path }}`

```
{% raw %}{% include list.liquid all=true %}{% endraw %}

{% include list.liquid all=true %}
```
