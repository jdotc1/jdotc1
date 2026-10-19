# Jeff

**Radiation oncologist · Physician-scientist · Security researcher**

I build and harden **open-source medical imaging software for Apple Silicon and ARM64**, with a focus on native macOS applications, MR imaging, and radiomics.

My work covers DICOM and MRI metadata, secure file handling, native build systems, and application inspection. I contribute fixes upstream and develop focused tools for imaging and research workflows.

## Selected projects

| Project | What it does | Availability |
| --- | --- | --- |
| [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) | Local metadata pseudonymization for MR, CT, and RTSTRUCT batches, with consistent UID remapping and structured reports. Native Apple Silicon app and Python engine. | [macOS preview](https://github.com/jdotc1/dicom-anonymizer#download-and-install-the-macos-app) |
| [SidecarCompare](https://github.com/jdotc1/SidecarCompare) | Compare MRI JSON sidecars with exact decimal differences, typed values, and documented units. Native SwiftUI app with a shared Swift core and CLI. | [Build from source](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) · [CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |
| [Prism Native MCP](https://github.com/jdotc1/prism-native-mcp) | Create supported GraphPad Prism tables, descriptive analyses, native graphs, layouts, and figure exports through a local MCP server. | [Version-pinned source preview](https://github.com/jdotc1/prism-native-mcp#install-and-connect) |

Current private development includes **AIRS**, which incorporates EntitlementDiff's entitlement-comparison functionality, and **MacScope**, a binary-analysis and reverse-engineering workbench for macOS.

## Selected merged contributions

| Area | Upstream work |
| --- | --- |
| **Apple Silicon and macOS builds** | **[dcm2niix](https://github.com/rordenlab/dcm2niix/pull/1043):** build-path handling and propagation of [architecture](https://github.com/rordenlab/dcm2niix/pull/1044), [SDK](https://github.com/rordenlab/dcm2niix/pull/1045), and [toolchain](https://github.com/rordenlab/dcm2niix/pull/1047) settings. **[ITK](https://github.com/InsightSoftwareConsortium/ITK/pull/6947):** target-architecture selection for FFTW SIMD defaults. **[MINC Toolkit](https://github.com/BIC-MNI/minc-toolkit-v2/pull/255):** forwarding macOS build settings to HDF5. |
| **Medical imaging security** | **[BIDScoin](https://github.com/Donders-Institute/bidscoin/pull/302)** and **[FastSurfer](https://github.com/Deep-MI/FastSurfer/pull/950):** safer path handling in imaging commands and link helpers. **[deid](https://github.com/pydicom/deid/pull/304):** owner-only defaults for new pixel-cleaner output directories. **[dicom-validator](https://github.com/pydicom/dicom-validator/pull/301):** filename escaping in HTML report headings. |
| **Imaging workflow reliability** | **[ANTsPy](https://github.com/ANTsX/ANTsPy/pull/924):** HTTP-status checks before caching downloaded test data. **[pyplastimatch](https://github.com/ImagingDataCommons/pyplastimatch/pull/15):** propagation of conversion and resampling process failures. |
| **Native Linux ARM64 testing** | Build and test coverage for **[FabIO](https://github.com/silx-kit/fabio/pull/675)**, **[connected-components-3d](https://github.com/seung-lab/connected-components-3d/pull/153)**, **[zarrs](https://github.com/zarrs/zarrs/pull/490)**, and **[fastremap](https://github.com/seung-lab/fastremap/pull/60)**. |
| **Software supply-chain tooling** | **[CycloneDX Core Java](https://github.com/CycloneDX/cyclonedx-core-java/pull/957):** detection of JSON and XML software bills of materials with leading whitespace. |

## Current upstream proposals

Open pull requests include:

- **Medical imaging security:** [dicom-rs](https://github.com/Enet4/dicom-rs/pull/845) UID path-safety checks; [pynetdicom](https://github.com/pydicom/pynetdicom/pull/1099) password redaction; [PlatiPy](https://github.com/pyplati/platipy/pull/322) API-key handling across redirects; [TorchIO](https://github.com/TorchIO-project/torchio/pull/1529) preservation of HTTPS on failed downloads.
- **Image and data integrity:** [dicom2nifti](https://github.com/icometrix/dicom2nifti/pull/167) temporal metadata preservation; [NiBabel](https://github.com/nipy/nibabel/pull/1568) NIfTI extension-length validation; [PyMedPhys](https://github.com/pymedphys/pymedphys/pull/2394) checksum enforcement under optimized Python; [MONAI](https://github.com/Project-MONAI/MONAI/pull/9177) download-publication failure handling.
- **Native builds and packaging:** [3D Slicer](https://github.com/Slicer/Slicer/pull/9478) macOS bundle hardening and Apple Silicon workflow documentation; [OpenJPEG](https://github.com/uclouvain/openjpeg/pull/1677) relocated macOS library lookup; native Linux ARM64 coverage for [scikit-image](https://github.com/scikit-image/scikit-image/pull/8359), [OME-Zarr](https://github.com/ome/ome-zarr-py/pull/704), and [Zarr](https://github.com/zarr-developers/zarr-python/pull/4525).
- **Security tooling:** [Semgrep](https://github.com/semgrep/semgrep/pull/11991) parameter-scope handling and [rule accuracy](https://github.com/semgrep/semgrep-rules/pull/4085); [Gitleaks](https://github.com/gitleaks/gitleaks/pull/2307) report preservation during validation; [XCP-D](https://github.com/PennLINC/xcp_d/pull/1640) fork-PR validation with read-only permissions.

**[Full contribution index →](CONTRIBUTIONS.md)** — additional contributions, verified status, and work incorporated through maintainer-authored follow-ups. Status checked on **19 October 2026**.

## Engineering approach

My security research combines source review, static binary analysis, and focused regression testing. I pay particular attention to untrusted image metadata, filesystem boundaries, credential handling, dependency provenance, and architecture-specific behavior.

I favor small, reviewable changes with explicit validation scope. For imaging tools, that means preserving numerical values and metadata, surfacing failures clearly, and documenting the limits of each workflow.

## Connect

Project READMEs include setup instructions, examples, and current limitations. Issues and pull requests are welcome for reproducible bugs, medical imaging workflows, and native Apple Silicon/ARM64 improvements.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
