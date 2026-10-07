# Release Notes

## [5.1.0](#)
- Dropped `stepanenko3/laravel-helpers` (it caps `laravel/framework` at ^12); `in_array_wildcard()` replaced with `Str::is()`
- Require PHP ^8.1

## [5.0.0](#)
- Nova 5 only (`laravel/nova: ^5.0`)
- Icons use Nova 5 `<Icon name>` API and Heroicons v2 names (`arrow-path`, `magnifying-glass`, `command-line`)
- Tool CSS no longer ships Tailwind preflight (it restyled the whole Nova UI)
- `dark:` styles follow Nova's theme switch (`.dark` class) instead of the OS setting
- Removed unused Inertia dev dependencies

## [4.4.0](#)
- Added `Stepanenko3\NovaCommandRunner\Traits\RunsArtisan`
- Update `run_by` assignment to use the `getArtisanRunByName` method

## [4.1.0](#)
- `Stepanenko3\NovaCommandRunner\CommandRunner` migrate to `Stepanenko3\NovaCommandRunner\CommandRunnerTool`

## [4.0.0](#)

- Compatible with Nova 4.0
- Drop compability with Nova 3
- Dark mode compatibility
- Responsive
- Use Nova Vue components
- Migrate to Vue 3 and Tailwind 3
- Bug fixes
