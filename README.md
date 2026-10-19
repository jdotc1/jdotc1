# Jeff

**Radiation oncologist · Physician-scientist · Security researcher**

I build and harden **open-source medical imaging software for Apple Silicon and ARM64**, with a focus on native macOS applications, MR imaging, and radiomics.

My work covers DICOM and MRI metadata, secure file handling, native build systems, and application inspection. I contribute fixes upstream and develop focused tools for imaging and research workflows.

## Selected projects

| Project | What it does | Availability |
| --- | --- | --- |
| [AIRS](https://github.com/jdotc1/AIRS-app) | Inspect bounded ARM64 Mach-O unwind evidence and compare app entitlements in a native macOS workspace, with checked scope and unresolved results shown explicitly. | [macOS preview](https://github.com/jdotc1/AIRS-app/releases/tag/v0.1.0) |
| [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) | Local metadata pseudonymization for MR, CT, and RTSTRUCT batches, with consistent UID remapping and structured reports. Native Apple Silicon app and Python engine. | [macOS preview](https://github.com/jdotc1/dicom-anonymizer#download-and-install-the-macos-app) |
| [SidecarCompare](https://github.com/jdotc1/SidecarCompare) | Compare MRI JSON sidecars with exact decimal differences, typed values, and documented units. Native SwiftUI app with a shared Swift core and CLI. | [Build from source](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) · [CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |
| [Prism Native MCP](https://github.com/jdotc1/prism-native-mcp) | Create supported GraphPad Prism tables, descriptive analyses, native graphs, layouts, and figure exports through a local MCP server. | [Version-pinned source preview](https://github.com/jdotc1/prism-native-mcp#install-and-connect) |

Other private development includes **MacScope**, a binary-analysis and reverse-engineering workbench for macOS.

## Selected merged contributions

Selected upstream merges focused on defensive input handling, protecting imaging outputs, and software supply-chain reliability.

| Focus | Merged upstream contribution |
| --- | --- |
| **Defensive NIfTI parsing** | **[NiBabel #1568](https://github.com/nipy/nibabel/pull/1568):** Rejects undersized NIfTI extensions before payload reads, avoiding unnecessary reads of the remaining input when processing malformed files. |
| **Privacy of imaging outputs** | **[deid #304](https://github.com/pydicom/deid/pull/304):** Defaults newly created pixel-cleaner output directories to owner-only permissions, reducing unintended access on shared POSIX systems. |
| **HTML report safety** | **[dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301):** Escapes filenames in HTML validation-report headings so filename content renders as text. |
| **Command-path hardening** | **[BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302):** Quotes image, output, and mask paths in local SynthStrip commands, keeping shell metacharacters in those paths literal. |
| **SBOM ingestion reliability** | **[CycloneDX Core Java #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957):** Corrects format detection for JSON/XML software bills of materials with leading whitespace, allowing valid SBOMs to reach the appropriate parser. |
| **Dependency reproducibility** | **[dcm2niix #1046](https://github.com/rordenlab/dcm2niix/pull/1046):** Pins the optional Cloudflare-zlib dependency to a fixed commit, making dependency source selection reproducible. |

Additional merged work covers native Apple Silicon/macOS builds, Linux ARM64 testing, and imaging workflow reliability; see the [full contribution index](CONTRIBUTIONS.md#merged-upstream-work).

## Current upstream proposals

Open pull requests include:

- **Medical imaging security:** [dicom-rs](https://github.com/Enet4/dicom-rs/pull/845) UID path-safety checks; [pynetdicom](https://github.com/pydicom/pynetdicom/pull/1099) password redaction; [PlatiPy](https://github.com/pyplati/platipy/pull/322) API-key handling across redirects; [TorchIO](https://github.com/TorchIO-project/torchio/pull/1529) preservation of HTTPS on failed downloads.
- **Image and data integrity:** [dicom2nifti](https://github.com/icometrix/dicom2nifti/pull/167) temporal metadata preservation; [PyMedPhys](https://github.com/pymedphys/pymedphys/pull/2394) checksum enforcement under optimized Python; [MONAI](https://github.com/Project-MONAI/MONAI/pull/9177) download-publication failure handling.
- **Native builds and packaging:** [3D Slicer](https://github.com/Slicer/Slicer/pull/9478) macOS bundle hardening and Apple Silicon workflow documentation; [OpenJPEG](https://github.com/uclouvain/openjpeg/pull/1677) relocated macOS library lookup; native Linux ARM64 coverage for [scikit-image](https://github.com/scikit-image/scikit-image/pull/8359), [OME-Zarr](https://github.com/ome/ome-zarr-py/pull/704), and [Zarr](https://github.com/zarr-developers/zarr-python/pull/4525).
- **Security tooling:** [Semgrep](https://github.com/semgrep/semgrep/pull/11991) parameter-scope handling and [rule accuracy](https://github.com/semgrep/semgrep-rules/pull/4085); [Gitleaks](https://github.com/gitleaks/gitleaks/pull/2307) report preservation during validation; [XCP-D](https://github.com/PennLINC/xcp_d/pull/1640) fork-PR validation with read-only permissions.

**[Full contribution index →](CONTRIBUTIONS.md)** — additional contributions, verified status, and work incorporated through maintainer-authored follow-ups. Status checked on **19 October 2026**.

## Engineering approach

My security research combines source review, static binary analysis, and focused regression testing. I pay particular attention to untrusted image metadata, filesystem boundaries, credential handling, dependency provenance, and architecture-specific behavior.

I favor small, reviewable changes with explicit validation scope. For imaging tools, that means preserving numerical values and metadata, surfacing failures clearly, and documenting the limits of each workflow.

## Connect

Project READMEs include setup instructions, examples, and current limitations. Issues and pull requests are welcome for reproducible bugs, medical imaging workflows, and native Apple Silicon/ARM64 improvements.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
