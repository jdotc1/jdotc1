# Jeff

**Radiation oncologist · Physician-scientist · Security researcher**

I work at the intersection of **medical imaging security, radiomics, and native macOS software on Apple Silicon (ARM64)**. I contribute defensive fixes to the open-source tools used to acquire, convert, analyze, and share imaging data, and build applications for inspecting binaries, reviewing entitlements, and preserving research data integrity.

My focus is practical: protect patient metadata and credentials, handle untrusted files safely, preserve quantitative imaging information, and make architecture-specific behavior explicit. My clinical and research interests in MR imaging and radiomics inform the problems I choose to work on.

## Applications I develop

| Application | Security and research focus | Explore |
| --- | --- | --- |
| **[AIRS](https://github.com/jdotc1/AIRS-app)** | Native macOS workspace for bounded ARM64 Mach-O unwind analysis and app-entitlement comparisons. Reads inspected binaries as data, with analysis coverage and unresolved results made explicit. | [Download the Apple Silicon preview](https://github.com/jdotc1/AIRS-app/releases) |
| **[EntitlementDiff](https://github.com/jdotc1/EntitlementDiff)** | Review changes in declared macOS app entitlements between builds, with explicit arm64 or x86_64 selection, exact typed values, and saved comparisons colleagues can reopen. Inspects the selected main executable without launching the app. | [Download the macOS app](https://github.com/jdotc1/EntitlementDiff/releases) |
| **[DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer)** | Local DICOM metadata pseudonymization for MR, CT, and RTSTRUCT batches. Consistently remaps patient-specific UIDs and references, audits staged outputs, and preserves source files. | [Download the Apple Silicon preview](https://github.com/jdotc1/dicom-anonymizer/releases) |
| **[SidecarCompare](https://github.com/jdotc1/SidecarCompare)** | Review MRI acquisition-metadata changes using exact decimal comparisons, typed values, and documented units. Preserves both source sidecars and supports local snapshots and reports through a native SwiftUI app and shared CLI core. | [Build the macOS app](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) · [Use the CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |

I also develop **MacScope**, a private binary-analysis and reverse-engineering workbench for macOS. My related research tooling includes **[Prism Native MCP](https://github.com/jdotc1/prism-native-mcp)**, which connects original observations to native GraphPad Prism tables, descriptive analyses, editable graphs, and layouts.

## Security contributions

My upstream work addresses concrete failure modes in imaging and research software: malformed input, shell interpretation of filenames, unintended file access, credential exposure, and unreliable dependency or download handling.

Selected merged upstream contributions:

| Area | Contribution |
| --- | --- |
| **Defensive image parsing** | [NiBabel #1568](https://github.com/nipy/nibabel/pull/1568): reject undersized NIfTI extensions before payload reads. [NIFTI-Reader-JS #58](https://github.com/rii-mango/NIFTI-Reader-JS/pull/58): reject negative NIfTI extension sizes before payload access. |
| **Privacy of imaging outputs** | [deid #304](https://github.com/pydicom/deid/pull/304): default newly created pixel-cleaner output directories to owner-only permissions. |
| **Safe report rendering** | [dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301): render filenames as text in HTML validation-report headings. |
| **macOS helper isolation** | [RSNA Anonymizer #41](https://github.com/RSNA/anonymizer/pull/41): place the compiled documentation helper in a private temporary directory for each process, avoiding reuse of a fixed-name executable. |
| **Literal command arguments** | [BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302): quote image, output, and mask paths in local SynthStrip commands. |
| **Reproducible dependency sources** | [dcm2niix #1046](https://github.com/rordenlab/dcm2niix/pull/1046): pin the optional Cloudflare zlib dependency to a fixed source commit. |
| **Security-tooling compatibility** | [CycloneDX Core Java #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957): recognize JSON/XML software bills of materials with leading whitespace. |

The **[full contribution index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md)** brings together my work across medical imaging and radiomics, DICOM and NIfTI infrastructure, native macOS builds, Linux ARM64 coverage, security tooling, and research workflows. It includes code contributions, documentation, issue reports, and fork work, organized by project.

## Engineering approach

I combine source review, static binary analysis, and focused regression testing. I pay particular attention to parser boundaries, filesystem containment, credential handling, dependency provenance, and the differences between declared configuration and observed behavior.

For imaging and radiomics, numerical values, units, acquisition metadata, and source lineage matter as much as successful execution. I favor small, reviewable fixes and local tools that preserve inputs, expose failures, and make their supported scope clear.

## Connect

I welcome collaboration on medical imaging security, radiomics infrastructure, defensive binary analysis, and native Apple Silicon applications. Project READMEs include setup instructions, examples, and supported workflows.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
