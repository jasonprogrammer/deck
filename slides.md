# Deck, a minimalist presentation tool

---

# Built with Rust

<div data-slide-classes="desert-sand"></div>

---

# Thanks to

- [pulldown_cmark](https://github.com/raphlinus/pulldown-cmark) (markdown to html)
- [syntect](https://github.com/trishume/syntect) (syntax highlighting)
- [warp](https://github.com/seanmonstar/warp) (local server)
- [inotify](https://github.com/inotify-rs/inotify) (automatic reload)

---

# Syntax highlighting

```rust
fn main() {
  // Read input from stdin
  let mut input = String::new();
  io::stdin().read_to_string(&mut input).unwrap();

  // Load syntax and theme
  let syntax_set = SyntaxSet::load_defaults_newlines();
  let theme_set = ThemeSet::load_defaults();
  let theme = &theme_set.themes["base16-ocean.dark"];
}
```

---

# List

1) First
2) Second
3) Third

---

# Bullet points

* First
* Second
* Third

---

# Tables

|Col1|Col2|Col3|
|----|----|----|
|Row11|Row12|Row13|
|Row21|Row22|Row23|

---

# Quote

> Be the change that you wish to see in the world.
