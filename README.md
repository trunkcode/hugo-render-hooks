# Hugo Seo

[Hugo](https://gohugo.io/) module adds the following attributes on the markup.

- `target` and `rel` attribute on external link
- `title` attribute on link and image elements
- Font Awesome external icon on external link (Need Font Awesome in theme)

## Install

```bash
hugo mod get github.com/trunkcode/hugo-seo@v0.1.0
```

## Add theme module configuration settings

Add the settings in the following snippet at the end of your site configuration file (default: config.toml) and save the file.

### config.toml

```toml
[module]
  [module.hugoVersion]
    extended = true
    min = "0.73.0"
  [[module.imports]]
    path = "github.com/trunkcode/hugo-seo"
    disable = false
```

### config.yaml

```yml
module:
  hugoVersion:
    extended: true
    min: 0.73.0
  imports:
    - path: github.com/trunkcode/hugo-seo
      disable: false
```

### config.json

```json
{
  "module": {
    "hugoVersion": {
      "extended": true,
      "min": "0.73.0"
    },
    "imports": [
      {
        "path": "github.com/trunkcode/hugo-seo",
        "disable": false
      }
    ]
  }
}
```

## Configuration

### Remove external icon from the link

#### params.toml

```toml
[hugoSeo]
  externalLinkIcon = false
```

#### params.yaml

```yml
hugoSeo:
  externalLinkIcon: false
```

#### params.json

```json
{
  "hugoSeo": {
    "externalLinkIcon": false
  }
}
```

## License ![GitHub](https://img.shields.io/github/license/trunkcode/hugo-seo)

This project is licensed under the Apache License 2.0 - see the [LICENSE.md](https://github.com/trunkcode/hugo-seo/blob/main/LICENSE) file for details.
