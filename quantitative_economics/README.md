# Quantitative Economics Template

Official LaTeX template for submissions to [Quantitative Economics (QE)](http://qeconomics.org/ojs/index.php/qe), a journal of the Econometric Society.

![](thumbnail.png)

## About

This template provides the official LaTeX style files and template for preparing manuscripts for submission to Quantitative Economics. As of 2024, the journal is an electronic publication only.

- **Publisher**: The Econometric Society
- **Website**: https://www.econometricsociety.org/
- **Submission Guidelines**: [QE Author Guidelines](https://www.econometricsociety.org/publications/quantitative-economics/authors)

## Features

- Supports submissions to all Econometric Society journals:
  - Quantitative Economics (QE)
  - Econometrica (ECTA)
  - Theoretical Economics (TE)
- Complete LaTeX style files (`econsocart.cls`, `econsocart.cfg`)
- BibTeX style for references (`qe.bst`)
- Pre-defined theorem environments and mathematical formatting
- Comprehensive author metadata support:
  - Multiple authors with affiliations
  - Corresponding author designation
  - Author notes and acknowledgments
- Support for JEL classification codes and keywords
- Draft mode with line numbers for initial submission
- Final mode for prepublication
- Citation styles: author-year (default) or numbered references

## Files Included

- `template.tex` - Main template file for article preparation
- `econsocart.cls` - LaTeX class file for Econometric Society journals
- `econsocart.cfg` - Configuration file for the class
- `qe.bst` - BibTeX style file for bibliography formatting
- `template.yml` - Template configuration for MyST
- `example.md` - Example document using this template

## Usage

### With MyST Markdown

1. Install required tools:
   ```bash
   npm install -g jtex
   pip install myst-parser
   ```

2. Create a new markdown file with frontmatter:
   ```yaml
   ---
   title: Your Article Title
   exports:
     - format: pdf
       template: .
       draft: true
   authors:
     - name: Author Name
       email: author@institution.edu
       affiliations:
         - Institution Name
   ---
   ```

3. Build your document:
   ```bash
   myst build article.md --pdf
   ```

### With LaTeX

1. Ensure you have a complete TeX distribution installed
2. Place the style files in your working directory:
   - `econsocart.cls`
   - `econsocart.cfg`
   - `qe.bst`
3. Use `template.tex` as your starting point
4. Compile with your preferred LaTeX engine (pdfLaTeX recommended)

## Template Options

The template supports several options that can be configured in your frontmatter or `template.yml`:

- `draft`: Boolean flag for draft mode (adds line numbers)
- `doc_class`: Journal selection (`qe`, `ecta`, or `te`)
- `style`: Citation style (`nameyear` or `number`)
- `font_size`: Base font size (`10pt`, `11pt`, `12pt`)
- `margin_size`: Margin size (`normal`, `wide`, `narrow`)

## Troubleshooting

- **Common Issues**: Ensure all required fields in `template.yml` are filled.
- **Compilation Errors**: Check for missing packages or incorrect LaTeX syntax.

## Example

See `example.md` for a complete sample document using this template.

## Contributing

This template is maintained as part of the MyST template collection. To contribute improvements:

1. Fork the repository
2. Make your changes
3. Submit a pull request

## Support

For template issues:
- Open an issue on GitHub
- Contact [latex-support@vtex.lt](mailto:latex-support@vtex.lt)

For journal submission questions:
- Contact the [Quantitative Economics Editorial Office](http://qeconomics.org/ojs/index.php/qe)

For additional resources and help:
- Visit the [MyST documentation](https://myst-parser.readthedocs.io/)
- Join the [MyST community discussions](https://github.com/orgs/myst-templates/discussions)
