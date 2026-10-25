**medical imaging security · radiation oncology**

I identify and patch security and data-integrity defects in medical imaging software, focusing on defensive DICOM/NIfTI parsing, de-identification integrity, archive containment, and filesystem safeguards. I extend this work to scientific infrastructure and develop open-source privacy, binary-inspection, and research tools for Apple Silicon (ARM64), informed by my background in radiation oncology, MR imaging, and radiomics.

## Medical imaging hardening

[**88 PRs merged** across **49 external repositories**](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md), spanning medical imaging, scientific data integrity, and platform engineering.

### Selected security & privacy contributions

#### Medical imaging & privacy

| Merged contributions |
| :--- |
| **Imaging parser hardening**<br>[NiBabel #1568](https://github.com/nipy/nibabel/pull/1568) and [NIFTI-Reader-JS #58](https://github.com/rii-mango/NIFTI-Reader-JS/pull/58): reject undersized NIfTI extensions before reading payloads.<br>[highdicom #471](https://github.com/ImagingDataCommons/highdicom/pull/471): reject undefined DICOM encapsulated pixel-fragment lengths before reading their payloads. |
| **Archive extraction containment**<br>[Nilearn #6654](https://github.com/nilearn/nilearn/pull/6654): validate extraction destinations by path components to prevent sibling-prefix confusion in containment checks. |
| **De-identification policy integrity**<br>[deid #306](https://github.com/pydicom/deid/pull/306): preserve earlier named filter rules so later recipes cannot silently replace them.<br>[deid #307](https://github.com/pydicom/deid/pull/307): refresh DICOM field lookups and apply KEEP rules to current fields, including newly added ones. |
| **Validation-state isolation**<br>[dicom-validator #303](https://github.com/pydicom/dicom-validator/pull/303): restore pydicom's process-wide reading-validation mode after success or failure so permissive settings do not persist. |
| **Medical imaging output permissions**<br>[deid #304](https://github.com/pydicom/deid/pull/304): default new pixel-cleaner output directories to owner-only permissions. |
| **HTML output encoding**<br>[dicom-validator #301](https://github.com/pydicom/dicom-validator/pull/301): escape filenames in HTML report headings to render markup as text. |
| **Temporary executable isolation**<br>[RSNA Anonymizer #41](https://github.com/RSNA/anonymizer/pull/41): isolate each process's compiled macOS documentation helper in a private temporary directory. |
| **Shell argument integrity**<br>[BIDScoin #302](https://github.com/Donders-Institute/bidscoin/pull/302): quote image, output, and mask paths in local SynthStrip commands. |
| **Supply chain reproducibility**<br>[dcm2niix #1046](https://github.com/rordenlab/dcm2niix/pull/1046): pin optional Cloudflare zlib to a source commit. |
| **Archive checksum enforcement**<br>[PyMedPhys #2394](https://github.com/pymedphys/pymedphys/pull/2394): enforce TRF archive checksums under Python `-O`; retain incoming logfiles when verification fails. |

#### Broader security & data-integrity engineering

| Merged contributions |
| :--- |
| **Unintended file overwrite prevention**<br>[fonttools #4342](https://github.com/fonttools/fonttools/pull/4342): protect unrelated ZIP archives during file generation.<br>[svglib #518](https://github.com/deeplook/svglib/pull/518): parse compressed SVGs without overwriting sibling files. |
| **S3 request integrity**<br>[s3fs #1067](https://github.com/fsspec/s3fs/pull/1067): forward delete safeguards, including expected bucket owner and MFA parameters.<br>[s3fs #1068](https://github.com/fsspec/s3fs/pull/1068): honor exclusive-create conditions, ACLs, and metadata for zero-byte writes. |
| **Array index bounds enforcement**<br>[PyTables #1389](https://github.com/PyTables/PyTables/pull/1389) and [#1393](https://github.com/PyTables/PyTables/pull/1393): reject invalid indices before data access, preventing unintended reads and writes. |
| **SFTP directory permissions**<br>[fsspec #2358](https://github.com/fsspec/filesystem_spec/pull/2358): honor requested permissions when creating parent directories. |
| **Code-signature evidence integrity**<br>[REA #5765](https://github.com/morluto/rea/pull/5765): preserve partial Mach-O signature observations and explicitly flag incomplete per-architecture coverage. |

### Open medical-imaging security proposals

These proposals remain **open and unmerged**; they are separate from the 88 merged PRs.

| Open hardening proposals |
| :--- |
| **Output-path containment**<br>[dicomweb-client #130](https://github.com/ImagingDataCommons/dicomweb-client/pull/130): propose constraining UID-derived CLI output paths to the selected directory. |
| **Credential redaction**<br>[MRIQC #1451](https://github.com/nipreps/mriqc/pull/1451): propose redacting NITRC credentials from failed-download diagnostics. |
| **Literal data parsing**<br>[HeuDiConv #880](https://github.com/nipy/heudiconv/pull/880): propose parsing cached conversion tables as data rather than executing expressions. |

## My projects

I develop and maintain these **MIT-licensed open-source projects**.

| Projects |
| :--- |
| **[DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer)**<br>Local macOS preview for pseudonymization of MR, CT, and RTSTRUCT metadata, with optional MRI JSON-sidecar cleaning. Bundles Python, consistently remaps patient-specific UIDs and references, audits output, and supports interruption recovery. Preserves source files; leaves image pixels and contours unchanged.<br>[Download](https://github.com/jdotc1/dicom-anonymizer/releases) |
| **[AIRS](https://github.com/jdotc1/AIRS)**<br>Native macOS evidence-review workspace for bounded ARM64 Mach-O unwind analysis, structural code-signature evidence, and entitlement comparisons. Inspects binaries as data without executing them; reports coverage and unresolved results.<br>[Download](https://github.com/jdotc1/AIRS/releases) |
| **[EntitlementDiff](https://github.com/jdotc1/EntitlementDiff)**<br>Read-only macOS security-review utility comparing declared entitlements across app builds and architectures, with exact typed values and saved comparisons. Inspects the selected main executable without launching the app; does not establish effective permissions.<br>[Download](https://github.com/jdotc1/EntitlementDiff/releases) |
| **[SidecarCompare](https://github.com/jdotc1/SidecarCompare)**<br>Compare MRI acquisition metadata with exact decimals, typed values, and documented units. Preserves source sidecars and saves local snapshots and reports through a native SwiftUI app and shared CLI core.<br>[Use CLI](https://github.com/jdotc1/SidecarCompare#command-line-comparison) |

My research tooling also includes **[Prism Native MCP](https://github.com/jdotc1/prism-native-mcp)**, connecting original observations to native GraphPad Prism tables, descriptive analyses, editable graphs, and layouts.

## Additional merged contributions

### Scientific data integrity and security tooling

| Merged contributions |
| :--- |
| **Array type and view integrity**<br>[PyTables #1387](https://github.com/PyTables/PyTables/pull/1387): preserve coordinate views and read-only indices.<br>[PyTables #1388](https://github.com/PyTables/PyTables/pull/1388): reject non-integer Atom dimensions before coercion. |
| **Atomic download publication**<br>[BrainStat #385](https://github.com/MICA-MNI/BrainStat/pull/385): publish downloads atomically after successful copying, preserving existing files on failure. |
| **Imaging metadata and geometry integrity**<br>[highdicom #487](https://github.com/ImagingDataCommons/highdicom/pull/487): return singleton DICOM structured-report temporal coordinates as sequences; preserve multi-value containers and element types.<br>[PyVista #9454](https://github.com/pyvista/pyvista/pull/9454): compare structured-data extents to distinguish cell layouts and shifted offsets. |
| **Metadata path integrity**<br>[ANTsPy #931](https://github.com/ANTsX/ANTsPy/pull/931): replace only the terminal `.npy` suffix to keep JSON sidecars beside NumPy images; document legacy-path migration. |
| **Session capability reporting**<br>[REA #5763](https://github.com/morluto/rea/pull/5763): align session-discovery capabilities with supported target operations. |
| **SBOM parser resilience**<br>[CycloneDX Core Java #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957): recognize JSON/XML SBOMs with leading whitespace. |
| **Security notification fidelity**<br>[Dependency-Track #7704](https://github.com/DependencyTrack/dependency-track/pull/7704): expose latest-version status in notification subjects. |

### Imaging, research, and ARM64 support

| Merged contributions |
| :--- |
| **Failure handling**<br>[Pillow #10271](https://github.com/python-pillow/Pillow/pull/10271): handle zero-width images in `ImageOps.cover()` without division by zero.<br>[ANTsPy #924](https://github.com/ANTsX/ANTsPy/pull/924): reject failed HTTP responses before caching test data.<br>[pyplastimatch #15](https://github.com/ImagingDataCommons/pyplastimatch/pull/15): propagate conversion and resampling failures to callers. |
| **Imaging build diagnostics**<br>[ITK #6987](https://github.com/InsightSoftwareConsortium/ITK/pull/6987): restore warnings for handwritten wrapper code while retaining suppression for generated sources. |
| **macOS architecture compatibility**<br>[ITK #6947](https://github.com/InsightSoftwareConsortium/ITK/pull/6947): derive FFTW SIMD defaults from the requested macOS architecture.<br>[dcm2niix #1043](https://github.com/rordenlab/dcm2niix/pull/1043): support linking from source paths containing spaces. |
| **Shell path safety**<br>[ITK-SNAP #280](https://github.com/pyushkevich/itksnap/pull/280): preserve spaced application paths in the macOS launcher.<br>[FastSurfer #950](https://github.com/Deep-MI/FastSurfer/pull/950): quote FreeSurfer stub destinations during helper generation. |
| **Buffering policy enforcement**<br>[fsspec #2359](https://github.com/fsspec/filesystem_spec/pull/2359): honor zero buffering for immediate and deferred SFTP opens. |
| **Linux ARM64 integration testing**<br>Cover JPEG/JPEG 2000 plugins and pydicom integration in [pylibjpeg-libjpeg #91](https://github.com/pydicom/pylibjpeg-libjpeg/pull/91) and [pylibjpeg-openjpeg #129](https://github.com/pydicom/pylibjpeg-openjpeg/pull/129).<br>Test the latest-Dask configuration in [OME-Zarr #704](https://github.com/ome/ome-zarr-py/pull/704).<br>Extend coverage to [zarrs #490](https://github.com/zarrs/zarrs/pull/490), [zarrs-python #199](https://github.com/zarrs/zarrs-python/pull/199), [connected-components-3d #153](https://github.com/seung-lab/connected-components-3d/pull/153), [fastremap #60](https://github.com/seung-lab/fastremap/pull/60), and [FabIO #675](https://github.com/silx-kit/fabio/pull/675). |
| **Test suite reliability**<br>[ITK #7004](https://github.com/InsightSoftwareConsortium/ITK/pull/7004): install xarray in macOS/Windows CI and mark its test skipped when the dependency is absent.<br>[Nilearn #6664](https://github.com/nilearn/nilearn/pull/6664): stabilize plotting-test parameter order for parallel collection.<br>[xarray #11780](https://github.com/pydata/xarray/pull/11780): skip the DataArray-to-Dask-DataFrame test when PyArrow is absent.<br>[silx #4745](https://github.com/silx-kit/silx/pull/4745): support Qt 6.12 drag-event constructors and older Qt versions. |

The **[full contribution index](https://github.com/jdotc1/jdotc1/blob/main/CONTRIBUTIONS.md)** links all merged PRs, documentation, issue reports, additional proposals, and fork work.

## Research & engineering practice

I use source review, static binary analysis, and focused regression tests to produce small, reviewable patches with reproducible evidence. My [AIRS](https://github.com/jdotc1/AIRS) project applies these principles to ARM64 Mach-O inspection, emphasizing bounded analysis, explicit coverage, and transparent reporting of unresolved findings. My [DICOM Anonymizer](https://github.com/jdotc1/dicom-anonymizer) documents a [private security-reporting process](https://github.com/jdotc1/dicom-anonymizer/blob/main/SECURITY.md) and guidance for synthetic reproductions.

In imaging and radiomics, I prioritize numerical fidelity, units, acquisition metadata, and source lineage, and distinguish declared configuration from observed behavior.

## Connect

I welcome collaboration on medical imaging security, radiomics infrastructure, defensive binary analysis, and native Apple Silicon applications.

[Research profile · ORCID](https://orcid.org/0009-0005-8244-8646)

