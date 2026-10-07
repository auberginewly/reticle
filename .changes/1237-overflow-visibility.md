### Fixed

- **`@reticlehq/browser` — text completely clipped by an overflow ancestor no longer counts as visible.** Expanding a clamped card now proves that its hidden paragraph became visible instead of returning `already_true`. Partly clipped content remains visible, including across shadow roots and slots; `inViewport` checks the portion surviving ancestor clipping. Closes [#1237](https://github.com/reticlehq/reticle/issues/1237).
