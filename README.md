# cocktailfyi

[![crates.io](https://img.shields.io/crates/v/cocktailfyi.svg)](https://crates.io/crates/cocktailfyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Cocktail recipes, ABV calculation, calorie estimation, and flavor profiling — API client for [cocktailfyi.com](https://cocktailfyi.com).

> **Try the interactive tools at [cocktailfyi.com](https://cocktailfyi.com)**

## Install

`cargo add cocktailfyi`

## Quick Start

```rust
use cocktailfyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("margarita").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install cocktailfyi` | [PyPI](https://pypi.org/project/cocktailfyi/) |
| **npm** | `npm install cocktailfyi` | [npm](https://www.npmjs.com/package/cocktailfyi) |
| **Go** | `go get github.com/fyipedia/cocktailfyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/cocktailfyi-go) |
| **Rust** | `cargo add cocktailfyi` | [crates.io](https://crates.io/crates/cocktailfyi) |
| **Ruby** | `gem install cocktailfyi` | [rubygems](https://rubygems.org/gems/cocktailfyi) |

## Embed Widget

Embed [CocktailFYI](https://cocktailfyi.com) widgets on any website with [cocktailfyi-embed](https://widget.cocktailfyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/cocktailfyi-embed@1/dist/embed.min.js"></script>
<div data-cocktailfyi="entity" data-slug="margarita"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.cocktailfyi.com)

## Links

- [CocktailFYI](https://cocktailfyi.com) — Main site
- [API Documentation](https://cocktailfyi.com/developers/)
- [OpenAPI Spec](https://cocktailfyi.com/api/openapi.json)
- [Glossary](https://cocktailfyi.com/glossary/)

## License

MIT
