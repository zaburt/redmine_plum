# Plum

A dark plum theme for Redmine (Redmine 7+) — near-black violet backgrounds,
deep plum panels and soft lilac accents, with orchid pink highlights.

## Installation

1. Clone this theme ([https://github.com/zaburt/redmine_plum](https://github.com/zaburt/redmine_plum)) into the Redmine `themes/`
   directory at the application root (Redmine 7+) as `plum`:

   ```
   git clone https://github.com/zaburt/redmine_plum.git themes/plum
   ```

   The result should contain:

   ```
   themes/plum/stylesheets/application.css
   ```

   > Note: Redmine 6 and earlier used `public/themes/` instead of `themes/`.

2. Restart Redmine so the new theme appears in the list of available themes.
   In production, precompile assets so the theme CSS/images are served:

   ```
   RAILS_ENV=production bin/rails assets:precompile
   ```

3. Go to `Administration -> Settings -> Display` and select "Plum" in the
   "Theme" drop-down list. Save your settings.

## Customize

1. Change `images/logo.svg` for the header/login logo and
   `favicon/favicon.svg` for the browser tab icon.
2. The palette is defined inline as hex values in
   `stylesheets/application.css`:

   | Role                  | Color     |
   |-----------------------|-----------|
   | Page background       | `#121114` |
   | Panel / box bg        | `#281D44` |
   | Raised / hover bg     | `#3E315F` |
   | Borders               | `#5C507D` |
   | Text                  | `#EAE4F7` |
   | Muted text            | `#A69DC0` |
   | Primary accent (lilac)| `#B89CFF` |
   | Secondary (orchid)    | `#E58FD6` |
   | Rose                  | `#D94F8C` |
   | Amber                 | `#D98A4A` |
   | Success               | `#3FA66B` |
   | Error                 | `#E05252` |

3. In production, re-run `assets:precompile` after editing any theme file.

## License

Licensed under [GNU GPLv2](LICENSE).

Copyright (c) 2026 Onur Küçük (onur [at] delipenguen.net)
