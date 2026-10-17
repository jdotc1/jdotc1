# Jeff

**Radiation oncologist · Physician-scientist · Independent developer**

I build native macOS tools and modernize medical imaging and scientific software for Apple silicon, with a focus on privacy, data integrity, and defensive security. My clinical practice and MR-based radiomics research guide this work, especially the need to preserve numerical behavior and handle sensitive imaging data carefully.

## Selected projects

| Project | When to use it | Get started |
| --- | --- | --- |
| [SidecarCompare](https://github.com/jdotc1/SidecarCompare) | Review MRI acquisition-metadata changes with exact decimal differences, typed values, and documented units. | [Build the macOS app or CLI](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) |
| [EntitlementDiff](https://github.com/jdotc1/EntitlementDiff) | Review changes in declared app entitlements between builds and share a comparison a colleague can reopen. | [Download the macOS app](https://github.com/jdotc1/EntitlementDiff/releases/latest) |
| [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) | Pseudonymize supported DICOM metadata across numeric patient-folder batches, with consistent UID remapping and a structured report. | [Standalone macOS preview and Python engine](https://github.com/jdotc1/dicom-anonymizer) |
| [Prism Native MCP](https://github.com/jdotc1/prism-native-mcp) | Create supported native GraphPad Prism tables, descriptive statistics, graphs, and layouts through MCP. | [Version-pinned source preview](https://github.com/jdotc1/prism-native-mcp) |

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

## Try, share, or contribute

Each project README explains its supported workflow, current availability, examples, and limits. If a tool fits your work, try its synthetic example, share the repository with a colleague, or open a focused issue with a reproducible example. For upstream contributions, the linked pull requests and contribution index show the current review record.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
