# Jeff

Radiation oncologist and security researcher building and hardening medical imaging software for ARM64 on macOS.

## Selected projects

| Project | When to use it | Get started |
| --- | --- | --- |
| [SidecarCompare](https://github.com/jdotc1/SidecarCompare) | Review changes between MRI JSON sidecars with exact decimal comparisons, typed values, and documented unit annotations. | [Build the macOS app](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) · [Use the CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |
| [EntitlementDiff](https://github.com/jdotc1/EntitlementDiff) | Compare declared app entitlements between builds and share saved comparisons that colleagues can reopen without the original apps. | [Download the macOS app](https://github.com/jdotc1/EntitlementDiff/releases/latest) |
| [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) | Pseudonymize supported DICOM metadata using numeric folder names as patient pseudonyms, with consistent UID remapping and a structured report. | [Install the macOS preview](https://github.com/jdotc1/dicom-anonymizer#download-and-install-the-macos-app) · [Try the Python engine](https://github.com/jdotc1/dicom-anonymizer#try-it-with-synthetic-data) |
| [Prism Native MCP](https://github.com/jdotc1/prism-native-mcp) | Create supported native GraphPad Prism tables, descriptive statistics, graphs, and layouts through MCP. | [Install the version-pinned source preview](https://github.com/jdotc1/prism-native-mcp#install-and-connect) |

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

Start with a project’s README for setup, synthetic examples, and current limitations. If a tool fits your work, try it, share the repository with a colleague, or open an issue with a reproducible example.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
