# rules-us-ak

Alaska state tax and benefit rules encoded in Cosilico DSL.

## Structure

```
rules-us-ak/
├── statutes/       # Alaska Statutes (AS)
│   └── akn/        # Akoma Ntoso XML format
├── regulations/    # Alaska Administrative Code (AAC)
└── README.md
```

## Akoma Ntoso Files

The `statutes/akn/` directory contains Alaska Statutes in [Akoma Ntoso](http://docs.oasis-open.org/legaldocml/akn-core/v1.0/akn-core-v1.0.html) XML format, an OASIS standard for legal document markup.

**Coverage:**
- 304 chapter files covering Titles 1-19
- Generated from akleg.gov on 2025-12-31
- Includes structured sections, subsections, and cross-references

**File naming:**
- `as-title-{TT}-chapter-{CC}.xml` - e.g., `as-title-43-chapter-23.xml` for Permanent Fund Dividends

## Sources

- **Alaska Statutes**: https://www.akleg.gov/basis/statutes.asp
- **Alaska Administrative Code**: https://www.akleg.gov/basis/aac.asp

## Usage

This repository is part of the Cosilico rules ecosystem. Rules are encoded from official Alaska state sources and can be compiled to multiple targets (Python, JavaScript, WASM, SQL).

## License

Rule encodings are open source. Original statute and regulation text is public domain.
