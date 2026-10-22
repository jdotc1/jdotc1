# Jeff

**Radiation oncologist · Physician-scientist · Security researcher**

I work at the intersection of **medical imaging security, radiomics, and native macOS software on Apple Silicon (ARM64)**. I contribute defensive fixes to the open-source tools used to acquire, convert, analyze, and share imaging data, and build applications for inspecting binaries, reviewing entitlements, and preserving research data integrity.

My focus is practical: protect patient metadata and credentials, handle untrusted files safely, preserve quantitative imaging information, and make architecture-specific behavior explicit. My clinical and research interests in MR imaging and radiomics inform the problems I choose to work on.

## My apps

| Application | Security and research focus | Explore |
| --- | --- | --- |
| **[AIRS](https://github.com/jdotc1/AIRS-app)** | Native macOS workspace for bounded ARM64 Mach-O unwind analysis and app-entitlement comparisons. Reads inspected binaries as data, with analysis coverage and unresolved results made explicit. | [Download the beta](https://github.com/jdotc1/AIRS-app/releases) |
| **[EntitlementDiff](https://github.com/jdotc1/EntitlementDiff)** | Review changes in declared macOS app entitlements between builds, with explicit arm64 or x86_64 selection, exact typed values, and saved comparisons colleagues can reopen. Inspects the selected main executable without launching the app. | [Download the macOS app](https://github.com/jdotc1/EntitlementDiff/releases) |
| **[DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer)** | Local DICOM metadata pseudonymization for MR, CT, and RTSTRUCT batches. Consistently remaps patient-specific UIDs and references, audits staged outputs, and preserves source files. | [Download the beta](https://github.com/jdotc1/dicom-anonymizer/releases) |
| **[SidecarCompare](https://github.com/jdotc1/SidecarCompare)** | Review MRI acquisition-metadata changes using exact decimal comparisons, typed values, and documented units. Preserves both source sidecars and supports local snapshots and reports through a native SwiftUI app and shared CLI core. | [Build the macOS app](https://github.com/jdotc1/SidecarCompare#build-and-run-on-a-mac) · [Use the CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |

I also develop **MacScope**, a private binary-analysis and reverse-engineering workbench for macOS. My related research tooling includes **[Prism Native MCP](https://github.com/jdotc1/prism-native-mcp)**, which connects original observations to native GraphPad Prism tables, descriptive analyses, editable graphs, and layouts.

## Upstream contributions

**39 merged pull requests across 29 upstream projects**, covering defensive input handling, research data integrity, imaging workflows, and platform support. The **[verified merge index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md#merged-upstream-contributions)** links every contribution to its upstream PR and separately documents **[three changes incorporated through maintainer-authored follow-ups](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md#changes-incorporated-through-maintainer-pull-requests)**.

### Security and data integrity

| Area | Selected merged contributions |
| --- | --- |
| **Defensive image parsing** | [NiBabel #1568](https://github.com/nipy/nibabel/pull/1568) and [NIFTI-Reader-JS #58](https://github.com/rii-mango/NIFTI-Reader-JS/pull/58): reject malformed NIfTI extension sizes before payload reads. [highdicom #471](https://github.com/ImagingDataCommons/highdicom/pull/471): reject undefined encapsulated pixel-fragment lengths before payload reads. |
| **Archive destination containment** | [Nilearn #6654](https://github.com/nilearn/nilearn/pull/6654): check path components so a sibling directory sharing a name prefix is not accepted as an extraction destination. |
| **Radiotherapy logfile integrity** | [PyMedPhys #2394](https://github.com/pymedphys/pymedphys/pull/2394): keep TRF archive checksum checks active under Python `-O`, preserving incoming logfiles when archived copies fail verification. |
| **Array data integrity** | [PyTables #1387](https://github.com/PyTables/PyTables/pull/1387), [#1388](https://github.com/PyTables/PyTables/pull/1388), and [#1389](https://github.com/PyTables/PyTables/pull/1389): preserve coordinate views and read-only indices, reject non-integer Atom dimensions, and validate selectors before conversion, reads, or writes. |
| **Privacy of imaging outputs** | [deid #304](https://github.com/pydicom/deid/pull/304): default newly created pixel-cleaner output directories to owner-only permissions. |
| **Safe report rendering** | [dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301): render filenames as text in HTML validation-report headings. |
| **macOS helper isolation** | [RSNA Anonymizer #41](https://github.com/RSNA/anonymizer/pull/41): place the compiled documentation helper in a private temporary directory for each process, avoiding reuse of a fixed-name executable. |
| **Literal command arguments** | [BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302): quote image, output, and mask paths in local SynthStrip commands. |
| **Reproducible dependency sources** | [dcm2niix #1046](https://github.com/rordenlab/dcm2niix/pull/1046): pin the optional Cloudflare zlib dependency to a fixed source commit. |
| **Security-tooling compatibility** | [CycloneDX Core Java #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957): recognize JSON/XML software bills of materials with leading whitespace. |

### Imaging, research, and platform support

| Area | Selected merged contributions |
| --- | --- |
| **Image processing and workflow reliability** | [Pillow #10271](https://github.com/python-pillow/Pillow/pull/10271): handle zero-width images in `ImageOps.cover()` without division by zero. [ANTsPy #924](https://github.com/ANTsX/ANTsPy/pull/924): reject failed HTTP responses before caching test data. [pyplastimatch #15](https://github.com/ImagingDataCommons/pyplastimatch/pull/15): propagate conversion and resampling failures to callers. |
| **macOS build compatibility** | [ITK #6947](https://github.com/InsightSoftwareConsortium/ITK/pull/6947): use the requested macOS target architecture for FFTW SIMD defaults. [dcm2niix #1043](https://github.com/rordenlab/dcm2niix/pull/1043): support linking from source paths containing spaces. Additional merged SDK, architecture, and toolchain fixes are recorded in the contribution index. |
| **Launcher and installation paths** | [ITK-SNAP #280](https://github.com/pyushkevich/itksnap/pull/280): preserve spaced application paths in the macOS launcher. [FastSurfer #950](https://github.com/Deep-MI/FastSurfer/pull/950): quote FreeSurfer stub destinations during helper generation. |
| **Binary-analysis evidence** | [REA #5765](https://github.com/morluto/rea/pull/5765): preserve mixed-slice Mach-O signature observations and partial evidence. [REA #5763](https://github.com/morluto/rea/pull/5763): align session-discovery capabilities with supported target operations. |
| **Native Linux ARM64 testing** | Add CI coverage to [zarrs #490](https://github.com/zarrs/zarrs/pull/490), [zarrs-python #199](https://github.com/zarrs/zarrs-python/pull/199), [connected-components-3d #153](https://github.com/seung-lab/connected-components-3d/pull/153), [fastremap #60](https://github.com/seung-lab/fastremap/pull/60), and [FabIO #675](https://github.com/silx-kit/fabio/pull/675). |
| **Test reliability** | [Nilearn #6664](https://github.com/nilearn/nilearn/pull/6664): stabilize plotting-test parameter order for parallel collection. [xarray #11780](https://github.com/pydata/xarray/pull/11780): guard a DataFrame-conversion test with its optional PyArrow dependency. |

The **[full contribution index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md)** also preserves documentation, issue reports, additional proposals, and fork work with links to the original records.

## Engineering approach

I combine source review, static binary analysis, and focused regression testing. I pay particular attention to parser boundaries, filesystem containment, credential handling, dependency provenance, and the differences between declared configuration and observed behavior.

For imaging and radiomics, numerical values, units, acquisition metadata, and source lineage matter as much as successful execution. I favor small, reviewable fixes and local tools that preserve inputs, expose failures, and make their supported scope clear.

## Connect

I welcome collaboration on medical imaging security, radiomics infrastructure, defensive binary analysis, and native Apple Silicon applications. Project READMEs include setup instructions, examples, and supported workflows.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)
