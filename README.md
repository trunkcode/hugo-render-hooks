# Hugo Seo

[Hugo](https://gohugo.io/) module adds the following attributes on the markup.

- `target` and `rel` attribute on external link
- `title` attribute on link and image elements
- [Add Font Awesome external icon using configuration](#faexternalicon)

## Install

```bash
hugo mod get github.com/trunkcode/hugo-seo@v0.2.1
```

## Add theme module configuration settings

Add the settings in the following snippet at the end of your site configuration file (default: config.toml) and save the file.

### config.toml

```toml
[module]
  [[module.imports]]
    path = "github.com/trunkcode/hugo-seo"
    disable = false
```

### config.yaml

```yml
module:
  imports:
    - path: github.com/trunkcode/hugo-seo
      disable: false
```

### config.json

```json
{
  "module": {
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

#### config.toml

```toml
[Params]
  [hugoSeo]
    faExternalIcon = true
    relValue = "noreferrer nofollow"
```

#### config.yaml

```yml
Params:
  hugoSeo:
    faExternalIcon: true
    relValue: "noreferrer nofollow"
```

#### config.json

```json
{
  "Params": {
    "hugoSeo": {
      "faExternalIcon": true,
      "relValue": "noreferrer nofollow"
    }
  }
}
```

## Configuration Settings

The following is the full list of **Hugo Seo** variables with their default value. Users may choose to override those values in their site config file(s).

### faExternalIcon

Default value: false

Add Font Awesome external icon on the external links.

### relValue

Default value: "noopener"

Specifies the relationship between the current document and the linked document.

## License ![GitHub](https://img.shields.io/github/license/trunkcode/hugo-seo)

This project is licensed under the Apache License 2.0 - see the [LICENSE.md](https://github.com/trunkcode/hugo-seo/blob/main/LICENSE) file for details.
