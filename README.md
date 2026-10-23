**Independent security researcher · Open-source maintainer · Radiation oncologist**

I investigate and repair security and data-integrity failures in **medical imaging and scientific software**, contribute fixes upstream, and maintain **open-source security and research tools for Apple Silicon (ARM64)**. My work focuses on defensive DICOM/NIfTI parsing, archive containment, private output permissions, safe report rendering, and preserving caller-requested safeguards.

I develop and maintain **AIRS, EntitlementDiff, DICOM Anonymizer, and SidecarCompare** for binary inspection, entitlement review, imaging-data privacy, and reproducible metadata analysis. My clinical work in radiation oncology and research in MR imaging and radiomics inform this engineering work.

## Security research and upstream track record

**64 authored pull requests merged across 43 external repositories**, verified **October 23, 2026**. These are PRs authored by `jdotc1` and merged into repositories owned by others. The total spans security hardening, scientific data integrity, imaging workflows, platform support, and test improvements.

The **[verified contribution index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md#merged-upstream-contributions)** links all **64 merged PRs** to their upstream records. **[Three additional contributions](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md#changes-incorporated-through-maintainer-pull-requests)** incorporated through maintainer-authored follow-ups are documented separately.

### Selected merged security and privacy contributions

| Area | Merged contributions |
| --- | --- |
| **Defensive DICOM and NIfTI parsing** | [NiBabel #1568](https://github.com/nipy/nibabel/pull/1568) and [NIFTI-Reader-JS #58](https://github.com/rii-mango/NIFTI-Reader-JS/pull/58): reject undersized NIfTI extension lengths before payload reads. [highdicom #471](https://github.com/ImagingDataCommons/highdicom/pull/471): reject undefined encapsulated pixel-fragment lengths before payload reads. |
| **Archive destination containment** | [Nilearn #6654](https://github.com/nilearn/nilearn/pull/6654): check path components so a sibling directory sharing a name prefix is not accepted as an extraction destination. |
| **Private output permissions** | [deid #304](https://github.com/pydicom/deid/pull/304): default newly created pixel-cleaner output directories to owner-only permissions. [fsspec #2358](https://github.com/fsspec/filesystem_spec/pull/2358): preserve caller-selected SFTP directory modes when creating parents. |
| **S3 request safeguards** | [s3fs #1067](https://github.com/fsspec/s3fs/pull/1067): forward caller-supplied delete options, including expected bucket owner and MFA parameters. [s3fs #1068](https://github.com/fsspec/s3fs/pull/1068): preserve exclusive-create conditions, requested ACLs, and metadata for zero-byte writes. |
| **Safe HTML report rendering** | [dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301): escape filenames in validation-report headings so filename markup is rendered as text. |
| **macOS helper isolation** | [RSNA Anonymizer #41](https://github.com/RSNA/anonymizer/pull/41): place the compiled documentation helper in a private temporary directory for each process, avoiding reuse of a fixed-name executable. |
| **Literal command arguments** | [BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302): quote image, output, and mask paths in local SynthStrip commands. |
| **Dependency provenance** | [dcm2niix #1046](https://github.com/rordenlab/dcm2niix/pull/1046): pin the optional Cloudflare zlib dependency to a fixed source commit. |
| **Radiotherapy logfile integrity** | [PyMedPhys #2394](https://github.com/pymedphys/pymedphys/pull/2394): keep TRF archive checksum checks active under Python `-O`, preserving incoming logfiles when archived copies fail verification. |

## Open-source projects I maintain

I maintain the following **MIT-licensed open-source projects**, with a focus on explicit analysis scope, reproducible results, and preserving source data.

| Application | Security and research focus | Explore |
| --- | --- | --- |
| **[AIRS](https://github.com/jdotc1/AIRS-app)** | Native macOS workspace for bounded ARM64 Mach-O unwind analysis and app-entitlement comparisons. Reads inspected binaries as data, with analysis coverage and unresolved results made explicit. | [Download the beta](https://github.com/jdotc1/AIRS-app/releases) |
| **[EntitlementDiff](https://github.com/jdotc1/EntitlementDiff)** | Review changes in declared macOS app entitlements between builds, with explicit architecture selection, exact typed values, and saved comparisons colleagues can reopen. Inspects the selected main executable without launching the app. | [Download the macOS app](https://github.com/jdotc1/EntitlementDiff/releases) |
| **[DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer)** | Local DICOM metadata pseudonymization for MR, CT, and RTSTRUCT batches. Consistently remaps patient-specific UIDs and references, audits staged outputs, and preserves source files. | [Download the beta](https://github.com/jdotc1/dicom-anonymizer/releases) |
| **[SidecarCompare](https://github.com/jdotc1/SidecarCompare)** | Review MRI acquisition-metadata changes using exact decimal comparisons, typed values, and documented units. Preserves both source sidecars and supports local snapshots and reports through a native SwiftUI app and shared CLI core. | [Build the macOS app](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) · [Use the CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |

I also develop **MacScope**, a private binary-analysis and reverse-engineering workbench for macOS. My related research tooling includes **[Prism Native MCP](https://github.com/jdotc1/prism-native-mcp)**, which connects original observations to native GraphPad Prism tables, descriptive analyses, editable graphs, and layouts.

## Additional upstream contributions

### Scientific data integrity and security tooling

| Area | Merged contributions |
| --- | --- |
| **Array data integrity** | [PyTables #1387](https://github.com/PyTables/PyTables/pull/1387), [#1388](https://github.com/PyTables/PyTables/pull/1388), and [#1389](https://github.com/PyTables/PyTables/pull/1389): preserve coordinate views and read-only indices, reject non-integer Atom dimensions, and validate selectors before conversion, reads, or writes. |
| **Download publication** | [BrainStat #385](https://github.com/MICA-MNI/BrainStat/pull/385): stage downloads and replace the destination only after a successful copy, preserving an existing file when copying fails. |
| **Existing-file preservation** | [fonttools #4342](https://github.com/fonttools/fonttools/pull/4342): stage archives beside the destination before replacement, preserving unrelated sibling ZIPs and existing output if archive creation fails. [svglib #518](https://github.com/deeplook/svglib/pull/518): parse compressed SVG input directly, preserving sibling SVG files and relative-image resolution. |
| **DICOM validation state** | [dicom-validator #303](https://github.com/pydicom/dicom-validator/pull/303): restore the caller's pydicom reading-validation mode after file validation, including exceptional exits. |
| **Imaging metadata paths** | [ANTsPy #931](https://github.com/ANTsX/ANTsPy/pull/931): keep JSON sidecars adjacent to NumPy images by replacing only the terminal `.npy` suffix, with migration guidance for legacy metadata paths. |
| **Binary-analysis evidence** | [REA #5765](https://github.com/morluto/rea/pull/5765): preserve mixed-slice Mach-O signature observations and partial evidence. [REA #5763](https://github.com/morluto/rea/pull/5763): align session-discovery capabilities with supported target operations. |
| **SBOM compatibility** | [CycloneDX Core Java #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957): recognize JSON/XML software bills of materials with leading whitespace. |
| **Security-tool notifications** | [Dependency-Track #7704](https://github.com/DependencyTrack/dependency-track/pull/7704): expose the latest project status in notification subjects. |

### Imaging, research, and platform support

| Area | Merged contributions |
| --- | --- |
| **Image processing and workflow reliability** | [Pillow #10271](https://github.com/python-pillow/Pillow/pull/10271): handle zero-width images in `ImageOps.cover()` without division by zero. [ANTsPy #924](https://github.com/ANTsX/ANTsPy/pull/924): reject failed HTTP responses before caching test data. [pyplastimatch #15](https://github.com/ImagingDataCommons/pyplastimatch/pull/15): propagate conversion and resampling failures to callers. |
| **macOS build compatibility** | [ITK #6947](https://github.com/InsightSoftwareConsortium/ITK/pull/6947): use the requested macOS target architecture for FFTW SIMD defaults. [dcm2niix #1043](https://github.com/rordenlab/dcm2niix/pull/1043): support linking from source paths containing spaces. Additional merged SDK, architecture, and toolchain fixes are recorded in the contribution index. |
| **Launcher and installation paths** | [ITK-SNAP #280](https://github.com/pyushkevich/itksnap/pull/280): preserve spaced application paths in the macOS launcher. [FastSurfer #950](https://github.com/Deep-MI/FastSurfer/pull/950): quote FreeSurfer stub destinations during helper generation. |
| **Filesystem behavior** | [fsspec #2359](https://github.com/fsspec/filesystem_spec/pull/2359): preserve explicitly requested zero buffering for immediate and deferred SFTP opens. |
| **Native Linux ARM64 testing** | Add JPEG and JPEG 2000 plugin coverage, including pydicom integration, in [pylibjpeg-libjpeg #91](https://github.com/pydicom/pylibjpeg-libjpeg/pull/91) and [pylibjpeg-openjpeg #129](https://github.com/pydicom/pylibjpeg-openjpeg/pull/129). Add CI coverage to [zarrs #490](https://github.com/zarrs/zarrs/pull/490), [zarrs-python #199](https://github.com/zarrs/zarrs-python/pull/199), [connected-components-3d #153](https://github.com/seung-lab/connected-components-3d/pull/153), [fastremap #60](https://github.com/seung-lab/fastremap/pull/60), and [FabIO #675](https://github.com/silx-kit/fabio/pull/675). |
| **Test reliability and compatibility** | [Nilearn #6664](https://github.com/nilearn/nilearn/pull/6664): stabilize plotting-test parameter order for parallel collection. [xarray #11780](https://github.com/pydata/xarray/pull/11780): guard a DataFrame-conversion test with its optional PyArrow dependency. [silx #4745](https://github.com/silx-kit/silx/pull/4745): support Qt 6.12 drag-event constructors while retaining compatibility with older Qt versions. |

The **[full contribution index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md)** also preserves documentation, issue reports, additional proposals, and fork work with links to the original records.

## Research and engineering practice

I combine source review, static binary analysis, and focused regression testing to trace failures to specific parsing, filesystem, process, or data-handling boundaries. I favor small, reviewable patches with explicit supported scope and reproducible evidence. My maintained [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) includes a documented [private security-reporting process](https://github.com/jdotc1/dicom-anonymizer/blob/main/SECURITY.md) and guidance for synthetic reproductions.

For imaging and radiomics, numerical values, units, acquisition metadata, and source lineage matter as much as successful execution. My tools preserve inputs, expose failures and unresolved results, and distinguish declared configuration from observed behavior.

## Connect

I welcome collaboration on medical imaging security, radiomics infrastructure, defensive binary analysis, and native Apple Silicon applications.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)

