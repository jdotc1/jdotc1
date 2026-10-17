# Jeff

**Radiation oncologist · Physician-scientist · Independent developer**

I build native macOS tools and modernize medical imaging and scientific software for Apple silicon, with a focus on privacy, data integrity, and defensive security. My clinical practice and MR-based radiomics research guide this work, especially the need to preserve numerical behavior and handle sensitive imaging data carefully.

## Selected projects

| Project | What it does | Availability |
| --- | --- | --- |
| [SidecarCompare](https://github.com/jdotc1/SidecarCompare) | Compares MRI JSON acquisition metadata, with typed differences, exact decimal arithmetic, and documented unit annotations. | Native macOS app and CLI · source |
| [EntitlementDiff](https://github.com/jdotc1/EntitlementDiff) | Compares embedded entitlement declarations in the main executable of two app builds for a chosen architecture, without launching the inspected apps. | Native macOS app and Swift library |
| [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) | Performs local metadata pseudonymization for MR, CT, and RTSTRUCT batches. | Python engine and macOS app preview |
| [Prism Native MCP](https://github.com/jdotc1/prism-native-mcp) | Connects MCP clients to supported GraphPad Prism tables, descriptive statistics, graphs, and layouts on macOS. | Version-pinned source preview |

I also develop **MacScope**, a private binary-analysis and reverse-engineering workbench for macOS.

## Selected open-source contributions

These examples link directly to upstream pull requests. Statuses were checked on **17 October 2026**.

| Contribution | Focus | Status |
| --- | --- | --- |
| [BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302) | Preserve literal image paths in local SynthStrip commands. | Merged |
| [deid #304](https://github.com/pydicom/deid/pull/304) | Default newly created pixel-cleaner output directories to owner-only permissions. | Merged |
| [dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301) | Escape filenames in HTML validation-report headings. | Merged |
| [Semgrep Rules #4085](https://github.com/semgrep/semgrep-rules/pull/4085) | Correct C# authorization-rule false positives for explicit authentication schemes. | Open |
| [pynetdicom #1099](https://github.com/pydicom/pynetdicom/pull/1099) | Redact user-identity passwords in standard DICOM association logs. | Open |
| [PlatiPy #322](https://github.com/pyplati/platipy/pull/322) | Strip a custom API-key header when redirects cross authentication boundaries. | Open |

[Explore the contribution index →](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md)

## Engineering approach

I trace how software handles untrusted input and sensitive data, develop focused patches, and verify behavior with synthetic regression cases. I document compatibility changes and validation limits, with particular attention to preserving scientific results and intended application behavior.

My work spans parser robustness, credential protection, file and archive handling, download integrity, and reliable builds for modern hardware.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
