# Selfie Documentation

This directory contains the AsciiDoc documentation for the Selfie plugin.

## Building Documentation

To build the documentation locally:

```bash
./gradlew :selfie-docs:asciidoctor
```

The generated HTML documentation will be available in `selfie-docs/build/docs/`.

## Viewing Documentation

After building, open `selfie-docs/build/docs/index.html` in your browser.

## Publishing

Documentation is automatically published to GitHub Pages when changes are pushed to the `master` or `main` branch via the `.github/workflows/publish-docs.yml` workflow.

The published documentation is available at: https://bertramdev.github.io/selfie/

## Structure

- `src/docs/asciidoc/index.adoc` - Main documentation page with quick start and configuration
- `src/docs/asciidoc/advanced.adoc` - Advanced usage guide with detailed examples

## Editing Documentation

Documentation is written in AsciiDoc format. Key conventions:

- Use `[source,groovy]` for Groovy code examples
- Use `[source,xml]` for GSP/XML examples
- Keep examples practical and complete
- Use the `:project-version:` attribute for version references
