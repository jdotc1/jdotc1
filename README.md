**medical imaging security · radiation oncology**

I investigate security and data-integrity defects in medical imaging and scientific software and contribute focused upstream fixes. My work centers on defensive DICOM/NIfTI parsing, archive containment, filesystem permissions, output encoding, and integrity checks.

I also build open-source binary inspection, privacy, and research tools for Apple Silicon (ARM64), informed by my clinical work in radiation oncology and research in MR imaging and radiomics.

## Medical imaging hardening

**88 PRs merged** across **49 external repositories**.

### Selected security & privacy contributions

| Area | Merged contributions |
| :--- | :--- |
| **Imaging parser hardening** | [NiBabel #1568](https://github.com/nipy/nibabel/pull/1568) and [NIFTI-Reader-JS #58](https://github.com/rii-mango/NIFTI-Reader-JS/pull/58): reject undersized NIfTI extensions before reading payloads.<br>[highdicom #471](https://github.com/ImagingDataCommons/highdicom/pull/471): reject undefined encapsulated pixel-fragment lengths before reading payloads. |
| **Archive extraction containment** | [Nilearn #6654](https://github.com/nilearn/nilearn/pull/6654): check extraction paths by component, excluding sibling directories with matching name prefixes. |
| **De-identification field consistency** | [deid #307](https://github.com/pydicom/deid/pull/307): refresh DICOM field lookups after dataset or extraction-option changes; apply KEEP rules to current fields, including newly added ones. |
| **Filesystem access controls** | [deid #304](https://github.com/pydicom/deid/pull/304): default new pixel-cleaner output directories to owner-only permissions.<br>[fsspec #2358](https://github.com/fsspec/filesystem_spec/pull/2358): honor requested SFTP permissions when creating parent directories. |
| **S3 request integrity** | [s3fs #1067](https://github.com/fsspec/s3fs/pull/1067): forward delete safeguards, including expected bucket owner and MFA parameters.<br>[s3fs #1068](https://github.com/fsspec/s3fs/pull/1068): honor exclusive-create conditions, ACLs, and metadata for zero-byte writes. |
| **HTML output encoding** | [dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301): escape filenames in HTML report headings to render markup as text. |
| **Temporary executable isolation** | [RSNA Anonymizer #41](https://github.com/RSNA/anonymizer/pull/41): isolate each process's compiled macOS documentation helper in a private temporary directory. |
| **Shell argument integrity** | [BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302): quote image, output, and mask paths in local SynthStrip commands. |
| **Supply chain reproducibility** | [dcm2niix #1046](https://github.com/rordenlab/dcm2niix/pull/1046): pin optional Cloudflare zlib to a source commit. |
| **Archive checksum enforcement** | [PyMedPhys #2394](https://github.com/pymedphys/pymedphys/pull/2394): enforce TRF archive checksums under Python `-O`; retain incoming logfiles when verification fails. |

## My projects

I develop and maintain these **MIT-licensed open-source projects**.

| Application | Security & research focus | Explore |
| :--- | :--- | :--- |
| **[AIRS](https://github.com/jdotc1/AIRS-app)** | Native macOS workspace for bounded ARM64 Mach-O unwind analysis and entitlement comparisons. Reads binaries as data and reports coverage and unresolved results. | [Download](https://github.com/jdotc1/AIRS-app/releases) |
| **[EntitlementDiff](https://github.com/jdotc1/EntitlementDiff)** | Compare declared macOS entitlements by architecture, with exact typed values and saved comparisons. Inspects the selected main executable without launching the app. | [Download](https://github.com/jdotc1/EntitlementDiff/releases) |
| **[DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer)** | Local macOS pseudonymization of MR, CT, and RTSTRUCT metadata, with optional MRI JSON-sidecar cleaning. Bundles Python, consistently remaps patient-specific UIDs and references, audits output, and supports interruption recovery. Preserves source files; leaves image pixels and contours unchanged. | [Download](https://github.com/jdotc1/dicom-anonymizer/releases) |
| **[SidecarCompare](https://github.com/jdotc1/SidecarCompare)** | Compare MRI acquisition metadata with exact decimals, typed values, and documented units. Preserves source sidecars and saves local snapshots and reports through a native SwiftUI app and shared CLI core. | [Use CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |

My research tooling also includes **[Prism Native MCP](https://github.com/jdotc1/prism-native-mcp)**, connecting original observations to native GraphPad Prism tables, descriptive analyses, editable graphs, and layouts.

## Additional merged contributions

### Scientific data integrity and security tooling

| Area | Merged contributions |
| :--- | :--- |
| **Array validation safeguards** | [PyTables #1387](https://github.com/PyTables/PyTables/pull/1387), [PyTables #1388](https://github.com/PyTables/PyTables/pull/1388), and [PyTables #1389](https://github.com/PyTables/PyTables/pull/1389): preserve coordinate views and read-only indices, reject non-integer Atom dimensions, and validate selectors before conversion, reads, or writes. |
| **Atomic download publication** | [BrainStat #385](https://github.com/MICA-MNI/BrainStat/pull/385): publish downloads atomically after successful copying, preserving existing files on failure. |
| **File overwrite prevention** | [fonttools #4342](https://github.com/fonttools/fonttools/pull/4342): stage archives beside the destination before replacement, protecting sibling ZIPs and existing output on failure.<br>[svglib #518](https://github.com/deeplook/svglib/pull/518): read compressed SVGs directly, preserving sibling files and relative-image resolution. |
| **Validation state isolation** | [dicom-validator #303](https://github.com/pydicom/dicom-validator/pull/303): restore the caller's pydicom reading-validation mode, including after exceptions. |
| **Imaging metadata and geometry integrity** | [highdicom #487](https://github.com/ImagingDataCommons/highdicom/pull/487): return singleton DICOM structured-report temporal coordinates as sequences; preserve multi-value containers and element types.<br>[PyVista #9454](https://github.com/pyvista/pyvista/pull/9454): compare structured-data extents to distinguish cell layouts and shifted offsets. |
| **Metadata path integrity** | [ANTsPy #931](https://github.com/ANTsX/ANTsPy/pull/931): replace only the terminal `.npy` suffix to keep JSON sidecars beside NumPy images; document legacy-path migration. |
| **Analysis evidence integrity** | [REA #5765](https://github.com/morluto/rea/pull/5765): preserve mixed-slice Mach-O signature observations and partial evidence.<br>[REA #5763](https://github.com/morluto/rea/pull/5763): align session-discovery capabilities with supported target operations. |
| **SBOM parser resilience** | [CycloneDX Core Java #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957): recognize JSON/XML SBOMs with leading whitespace. |
| **Security notification fidelity** | [Dependency-Track #7704](https://github.com/DependencyTrack/dependency-track/pull/7704): expose latest-version status in notification subjects. |

### Imaging, research, and ARM64 support

| Area | Merged contributions |
| :--- | :--- |
| **Failure handling** | [Pillow #10271](https://github.com/python-pillow/Pillow/pull/10271): handle zero-width images in `ImageOps.cover()` without division by zero.<br>[ANTsPy #924](https://github.com/ANTsX/ANTsPy/pull/924): reject failed HTTP responses before caching test data.<br>[pyplastimatch #15](https://github.com/ImagingDataCommons/pyplastimatch/pull/15): propagate conversion and resampling failures to callers. |
| **Imaging build diagnostics** | [ITK #6987](https://github.com/InsightSoftwareConsortium/ITK/pull/6987): restore warnings for handwritten wrapper code while retaining suppression for generated sources. |
| **macOS architecture compatibility** | [ITK #6947](https://github.com/InsightSoftwareConsortium/ITK/pull/6947): derive FFTW SIMD defaults from the requested macOS architecture.<br>[dcm2niix #1043](https://github.com/rordenlab/dcm2niix/pull/1043): support linking from source paths containing spaces. |
| **Shell path safety** | [ITK-SNAP #280](https://github.com/pyushkevich/itksnap/pull/280): preserve spaced application paths in the macOS launcher.<br>[FastSurfer #950](https://github.com/Deep-MI/FastSurfer/pull/950): quote FreeSurfer stub destinations during helper generation. |
| **Buffering policy enforcement** | [fsspec #2359](https://github.com/fsspec/filesystem_spec/pull/2359): honor zero buffering for immediate and deferred SFTP opens. |
| **Linux ARM64 integration testing** | Cover JPEG/JPEG 2000 plugins and pydicom integration in [pylibjpeg-libjpeg #91](https://github.com/pydicom/pylibjpeg-libjpeg/pull/91) and [pylibjpeg-openjpeg #129](https://github.com/pydicom/pylibjpeg-openjpeg/pull/129).<br>Test the latest-Dask configuration in [OME-Zarr #704](https://github.com/ome/ome-zarr-py/pull/704).<br>Extend coverage to [zarrs #490](https://github.com/zarrs/zarrs/pull/490), [zarrs-python #199](https://github.com/zarrs/zarrs-python/pull/199), [connected-components-3d #153](https://github.com/seung-lab/connected-components-3d/pull/153), [fastremap #60](https://github.com/seung-lab/fastremap/pull/60), and [FabIO #675](https://github.com/silx-kit/fabio/pull/675). |
| **Test suite reliability** | [ITK #7004](https://github.com/InsightSoftwareConsortium/ITK/pull/7004): install xarray in macOS/Windows CI and mark its test skipped when the dependency is absent.<br>[Nilearn #6664](https://github.com/nilearn/nilearn/pull/6664): stabilize plotting-test parameter order for parallel collection.<br>[xarray #11780](https://github.com/pydata/xarray/pull/11780): skip the DataArray-to-Dask-DataFrame test when PyArrow is absent.<br>[silx #4745](https://github.com/silx-kit/silx/pull/4745): support Qt 6.12 drag-event constructors and older Qt versions. |

The **[full contribution index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md)** links all merged PRs, documentation, issue reports, additional proposals, and fork work.

## Research & engineering practice

I use source review, static binary analysis, and focused regression tests to produce small, reviewable patches with reproducible evidence. My [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) documents a [private security-reporting process](https://github.com/jdotc1/dicom-anonymizer/blob/main/SECURITY.md) and guidance for synthetic reproductions.

In imaging and radiomics, I prioritize numerical fidelity, units, acquisition metadata, and source lineage, and distinguish declared configuration from observed behavior.

## Connect

I welcome collaboration on medical imaging security, radiomics infrastructure, defensive binary analysis, and native Apple Silicon applications.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)

