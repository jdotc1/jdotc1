# Contribution index

Contributions to medical imaging, native macOS and ARM64 builds, defensive security, and research software.

[Back to my profile](https://github.com/jdotc1)

Public pull-request and issue statuses were checked on **19 October 2026**. Merged entries have been integrated into an upstream branch; release inclusion depends on the project. Open entries are proposals. The linked records provide current status, implementation details, and validation scope.

[Merged work](#merged-upstream-work) · [Open proposals](#open-upstream-proposals) · [Maintainer follow-ups](#work-incorporated-by-maintainers) · [Issue reports](#public-issue-reports) · [Fork work](#work-published-in-forks) · [Closed proposals](#closed-proposals)

## Merged upstream work

| Project | Scope of work | Record |
| --- | --- | --- |
| [ANTsPy](https://github.com/ANTsX/ANTsPy) | HTTP status checks before caching downloaded test data. | [PR #924](https://github.com/ANTsX/ANTsPy/pull/924) |
| [BIDScoin](https://github.com/Donders-Institute/bidscoin) | Literal image paths in local SynthStrip commands. | [PR #302](https://github.com/Donders-Institute/bidscoin/pull/302) |
| [connected-components-3d](https://github.com/seung-lab/connected-components-3d) | Native Linux ARM64 CI using the existing connected-component tests. | [PR #153](https://github.com/seung-lab/connected-components-3d/pull/153) |
| [CycloneDX](https://github.com/CycloneDX/cyclonedx-core-java) | Detection of JSON and XML software bills of materials with leading whitespace. | [PR #957](https://github.com/CycloneDX/cyclonedx-core-java/pull/957) |
| [dcm2niix](https://github.com/rordenlab/dcm2niix) | macOS build-path quoting, architecture/SDK/toolchain propagation, optional dependency source pinning, and explicit LTO settings. | [PR #1043](https://github.com/rordenlab/dcm2niix/pull/1043) · [PR #1044](https://github.com/rordenlab/dcm2niix/pull/1044) · [PR #1045](https://github.com/rordenlab/dcm2niix/pull/1045) · [PR #1046](https://github.com/rordenlab/dcm2niix/pull/1046) · [PR #1047](https://github.com/rordenlab/dcm2niix/pull/1047) · [PR #1048](https://github.com/rordenlab/dcm2niix/pull/1048) |
| [dcmqi](https://github.com/QIICR/dcmqi) | Support for macOS SDK names in CMAKE_OSX_SYSROOT. | [PR #566](https://github.com/QIICR/dcmqi/pull/566) |
| [deid](https://github.com/pydicom/deid) | Owner-only permissions by default for newly created pixel-cleaner output directories. | [PR #304](https://github.com/pydicom/deid/pull/304) |
| [dicom-validator](https://github.com/pydicom/dicom-validator) | Escaped filenames in HTML validation-report headings. | [PR #301](https://github.com/pydicom/dicom-validator/pull/301) |
| [FabIO](https://github.com/silx-kit/fabio) | Native Linux ARM64 package build and test CI. | [PR #675](https://github.com/silx-kit/fabio/pull/675) |
| [fastremap](https://github.com/seung-lab/fastremap) | Native Linux ARM64 CI and Windows editable-build compiler selection. | [PR #60](https://github.com/seung-lab/fastremap/pull/60) |
| [FastSurfer](https://github.com/Deep-MI/FastSurfer) | Quoted paths when generating FreeSurfer stub links. | [PR #950](https://github.com/Deep-MI/FastSurfer/pull/950) |
| [ITK](https://github.com/InsightSoftwareConsortium/ITK) | macOS target-architecture selection for FFTW SIMD defaults. | [PR #6947](https://github.com/InsightSoftwareConsortium/ITK/pull/6947) |
| [minc-toolkit-v2](https://github.com/BIC-MNI/minc-toolkit-v2) | Propagation of macOS build settings to HDF5. | [PR #255](https://github.com/BIC-MNI/minc-toolkit-v2/pull/255) |
| [NiBabel](https://github.com/nipy/nibabel) | Rejection of undersized NIfTI extensions before payload reads, avoiding unnecessary reads of malformed input. | [PR #1568](https://github.com/nipy/nibabel/pull/1568) |
| [PaperBanana](https://github.com/dwzhu-pku/PaperBanana) | Legacy plot routing and figure-sizing fixes, plus optional visual-metaphor planning for diagrams. | [PR #69](https://github.com/dwzhu-pku/PaperBanana/pull/69) · [PR #71](https://github.com/dwzhu-pku/PaperBanana/pull/71) |
| [pyplastimatch](https://github.com/ImagingDataCommons/pyplastimatch) | Propagation of conversion and resampling process failures. | [PR #15](https://github.com/ImagingDataCommons/pyplastimatch/pull/15) |
| [RSNA Anonymizer](https://github.com/RSNA/anonymizer) | Per-process macOS documentation helper caches. | [PR #41](https://github.com/RSNA/anonymizer/pull/41) |
| [zarrs](https://github.com/zarrs/zarrs) | Native Linux ARM64 CI using the existing Rust tests with all features enabled. | [PR #490](https://github.com/zarrs/zarrs/pull/490) |

## Open upstream proposals

| Project | Scope of work | Record |
| --- | --- | --- |
| [3D Slicer](https://github.com/Slicer/Slicer) | macOS bundle packaging failure checks, path containment, and ARM64 workflow documentation. | [PR #9478](https://github.com/Slicer/Slicer/pull/9478) |
| [batchgenerators](https://github.com/MIC-DKFZ/batchgenerators) | Scale sampling that respects requested intervals entirely below one. | [PR #144](https://github.com/MIC-DKFZ/batchgenerators/pull/144) |
| [Blosc / python-blosc2](https://github.com/Blosc/python-blosc2) | Native Linux ARM64 test coverage. | [PR #737](https://github.com/Blosc/python-blosc2/pull/737) |
| [BrainIAK](https://github.com/brainiak/brainiak) | Literal parsing of noise dictionaries. | [PR #616](https://github.com/brainiak/brainiak/pull/616) |
| [BrainStat](https://github.com/MICA-MNI/BrainStat) | Publication of downloaded data only after a successful copy. | [PR #385](https://github.com/MICA-MNI/BrainStat/pull/385) |
| [Clinica](https://github.com/aramis-lab/clinica) | Literal FreeSurfer atlas paths in subprocess arguments. | [PR #1741](https://github.com/aramis-lab/clinica/pull/1741) |
| [dcmjs](https://github.com/dcmjs-org/dcmjs) | Byte-count validation before BufferStream reads. | [PR #605](https://github.com/dcmjs-org/dcmjs/pull/605) |
| [dcmstack](https://github.com/moloney/dcmstack) | Independent metadata-filter defaults for each call. | [PR #102](https://github.com/moloney/dcmstack/pull/102) |
| [deep-mr](https://github.com/INFN-MRI/deep-mr) | Explicit rejection of MPS before CUDA conversion. | [PR #5](https://github.com/INFN-MRI/deep-mr/pull/5) |
| [Dependency-Track](https://github.com/DependencyTrack/dependency-track) | Latest-project status in notification subjects. | [PR #7704](https://github.com/DependencyTrack/dependency-track/pull/7704) |
| [dicom-numpy](https://github.com/innolitics/dicom-numpy) | Streamed reads of zipped DICOM members. | [PR #40](https://github.com/innolitics/dicom-numpy/pull/40) |
| [DICOM-rs](https://github.com/Enet4/dicom-rs) | UID path-safety checks before storing received DICOM files. | [PR #845](https://github.com/Enet4/dicom-rs/pull/845) |
| [dicom2nifti](https://github.com/icometrix/dicom2nifti) | Preservation of temporal zoom and time units during 4D NIfTI image reorientation. | [PR #167](https://github.com/icometrix/dicom2nifti/pull/167) |
| [dicomParser](https://github.com/cornerstonejs/dicomParser) | Validation of ByteStream seek bounds and integer offsets. | [PR #285](https://github.com/cornerstonejs/dicomParser/pull/285) |
| [dicomweb-client](https://github.com/ImagingDataCommons/dicomweb-client) | Containment of UID-derived CLI output paths. | [PR #130](https://github.com/ImagingDataCommons/dicomweb-client/pull/130) |
| [DIPY](https://github.com/dipy/dipy) | Dataset MD5 checksums in restricted Python runtimes. | [PR #4234](https://github.com/dipy/dipy/pull/4234) |
| [DLTK](https://github.com/DLTK/DLTK) | TAR member validation for IXI dataset extraction. | [PR #70](https://github.com/DLTK/DLTK/pull/70) |
| [FAE](https://github.com/salan668/FAE) | Folder-opening commands without shell interpretation. | [PR #73](https://github.com/salan668/FAE/pull/73) |
| [FreeSurfer](https://github.com/freesurfer/freesurfer) | SynthStrip Docker arguments passed without a shell. | [PR #1485](https://github.com/freesurfer/freesurfer/pull/1485) |
| [Gitleaks](https://github.com/gitleaks/gitleaks) | Preservation of existing reports during report-option validation. | [PR #2307](https://github.com/gitleaks/gitleaks/pull/2307) |
| [HD-BET](https://github.com/MIC-DKFZ/HD-BET) | Private staging for checkpoint downloads. | [PR #71](https://github.com/MIC-DKFZ/HD-BET/pull/71) |
| [HeuDiConv](https://github.com/nipy/heudiconv) | Literal parsing of cached conversion tables. | [PR #880](https://github.com/nipy/heudiconv/pull/880) |
| [highdicom](https://github.com/ImagingDataCommons/highdicom) | Validation of undefined pixel-fragment lengths before reads. | [PR #471](https://github.com/ImagingDataCommons/highdicom/pull/471) |
| [ImageIO](https://github.com/imageio/imageio) | Debug logging for FreeImage loader failures. | [PR #1240](https://github.com/imageio/imageio/pull/1240) |
| [InVesalius](https://github.com/invesalius/invesalius3) | TLS verification and bounded update-discovery requests. | [PR #1514](https://github.com/invesalius/invesalius3/pull/1514) |
| [ITK-SNAP](https://github.com/pyushkevich/itksnap) | Quoted application paths in the macOS launcher. | [PR #280](https://github.com/pyushkevich/itksnap/pull/280) |
| [libjxl](https://github.com/libjxl/libjxl) | Native Linux ARM64 static release workflow; documentation of an ARM64 GCC build workaround. | [PR #5039](https://github.com/libjxl/libjxl/pull/5039) · [PR #5040](https://github.com/libjxl/libjxl/pull/5040) |
| [medicaldetectiontoolkit](https://github.com/MIC-DKFZ/medicaldetectiontoolkit) | Literal checkpoint paths for cleanup. | [PR #151](https://github.com/MIC-DKFZ/medicaldetectiontoolkit/pull/151) |
| [MedPy](https://github.com/loli/medpy) | Version-specific Boost.Python library selection on macOS. | [PR #140](https://github.com/loli/medpy/pull/140) |
| [MIRTK](https://github.com/BioMedIA/MIRTK) | Apple silicon MATLAB MEX extension fallback. | [PR #793](https://github.com/BioMedIA/MIRTK/pull/793) |
| [MONAI](https://github.com/Project-MONAI/MONAI) | Propagation of download-publication failures. | [PR #9177](https://github.com/Project-MONAI/MONAI/pull/9177) |
| [MONAI Label](https://github.com/Project-MONAI/MONAILabel) | HTTP status checks before caching OpenID discovery responses. | [PR #1923](https://github.com/Project-MONAI/MONAILabel/pull/1923) |
| [MRIQC](https://github.com/nipreps/mriqc) | Credential redaction in NITRC download failures. | [PR #1451](https://github.com/nipreps/mriqc/pull/1451) |
| [napari / npe2](https://github.com/napari/npe2) | Native Linux ARM64 test coverage for the plugin infrastructure. | [PR #525](https://github.com/napari/npe2/pull/525) |
| [netneurotools](https://github.com/netneurolab/netneurotools) | Explicit TAR extraction filters for downloaded archives. | [PR #186](https://github.com/netneurolab/netneurotools/pull/186) |
| [neuromaps](https://github.com/netneurolab/neuromaps) | Literal paths in Workbench resampling. | [PR #226](https://github.com/netneurolab/neuromaps/pull/226) |
| [NIFTI-Reader-JS](https://github.com/rii-mango/NIFTI-Reader-JS) | Validation of negative NIfTI extension lengths before payload access. | [PR #58](https://github.com/rii-mango/NIFTI-Reader-JS/pull/58) |
| [NiftyReg](https://github.com/KCL-BMEIS/niftyreg) | SIMD selection for explicit macOS ARM64 targets. | [PR #155](https://github.com/KCL-BMEIS/niftyreg/pull/155) |
| [NiftySeg](https://github.com/KCL-BMEIS/NiftySeg) | Propagation of macOS target architectures to the optional NiftyReg build. | [PR #18](https://github.com/KCL-BMEIS/NiftySeg/pull/18) |
| [Nilearn](https://github.com/nilearn/nilearn) | Archive destination containment checks by path components and deterministic plotting-test parameter order. | [PR #6654](https://github.com/nilearn/nilearn/pull/6654) · [PR #6664](https://github.com/nilearn/nilearn/pull/6664) |
| [NiPy](https://github.com/nipy/nipy) | MATLAB launch without an intermediate shell. | [PR #591](https://github.com/nipy/nipy/pull/591) |
| [Nipype](https://github.com/nipy/nipype) | Executable dependency inspection without shell parsing; optional recursive globbing in SelectFiles. | [PR #3784](https://github.com/nipy/nipype/pull/3784) · [PR #3785](https://github.com/nipy/nipype/pull/3785) |
| [NiReports](https://github.com/nipreps/nireports) | Bounded scanning of embedded PNG data in SVG input. | [PR #292](https://github.com/nipreps/nireports/pull/292) |
| [nitrain](https://github.com/nitrain/nitrain) | OpenNeuro download destinations within the data root. | [PR #125](https://github.com/nitrain/nitrain/pull/125) |
| [NiWorkflows](https://github.com/nipreps/niworkflows) | Removal of an unused FreeSurfer helper. | [PR #1067](https://github.com/nipreps/niworkflows/pull/1067) |
| [nnU-Net](https://github.com/MIC-DKFZ/nnUNet) | Private staging for model installation downloads. | [PR #3078](https://github.com/MIC-DKFZ/nnUNet/pull/3078) |
| [Numcodecs](https://github.com/zarr-developers/numcodecs) | Native Linux ARM64 CI for the pinned Zarr integration case. | [PR #877](https://github.com/zarr-developers/numcodecs/pull/877) |
| [OME-Zarr](https://github.com/ome/ome-zarr-py) | Native Linux ARM64 CI using the existing latest-Dask test configuration. | [PR #704](https://github.com/ome/ome-zarr-py/pull/704) |
| [ome-zarr-models-py](https://github.com/ome-zarr-py/ome-zarr-models-py) | Native Linux ARM64 CI for metadata and coordinate-transformation tests. | [PR #484](https://github.com/ome-zarr-py/ome-zarr-models-py/pull/484) |
| [OpenJPEG](https://github.com/uclouvain/openjpeg) | Executable-relative library lookup for relocated macOS command-line tools. | [PR #1677](https://github.com/uclouvain/openjpeg/pull/1677) |
| [Papaya](https://github.com/rii-mango/Papaya) | Literal rendering of image title labels. | [PR #244](https://github.com/rii-mango/Papaya/pull/244) |
| [PlatiPy](https://github.com/pyplati/platipy) | Download safeguards, credential and service-log protections, upload/UID validation, DICOM receive isolation, and process/task failure handling. | [PR #316](https://github.com/pyplati/platipy/pull/316) · [PR #317](https://github.com/pyplati/platipy/pull/317) · [PR #318](https://github.com/pyplati/platipy/pull/318) · [PR #319](https://github.com/pyplati/platipy/pull/319) · [PR #320](https://github.com/pyplati/platipy/pull/320) · [PR #321](https://github.com/pyplati/platipy/pull/321) · [PR #322](https://github.com/pyplati/platipy/pull/322) · [PR #323](https://github.com/pyplati/platipy/pull/323) · [PR #324](https://github.com/pyplati/platipy/pull/324) · [PR #325](https://github.com/pyplati/platipy/pull/325) · [PR #326](https://github.com/pyplati/platipy/pull/326) · [PR #327](https://github.com/pyplati/platipy/pull/327) · [PR #328](https://github.com/pyplati/platipy/pull/328) · [PR #329](https://github.com/pyplati/platipy/pull/329) · [PR #330](https://github.com/pyplati/platipy/pull/330) |
| [pydantic-zarr](https://github.com/zarr-developers/pydantic-zarr) | Native Linux ARM64 metadata test coverage. | [PR #182](https://github.com/zarr-developers/pydantic-zarr/pull/182) |
| [pydicom](https://github.com/pydicom/pydicom) | HTTP status checks before writing downloaded data. | [PR #2390](https://github.com/pydicom/pydicom/pull/2390) |
| [pylibjpeg-libjpeg](https://github.com/pydicom/pylibjpeg-libjpeg) | Native Linux ARM64 CI for the JPEG plugin. | [PR #91](https://github.com/pydicom/pylibjpeg-libjpeg/pull/91) |
| [pylibjpeg-openjpeg](https://github.com/pydicom/pylibjpeg-openjpeg) | Native Linux ARM64 source-build and unit-test CI, including pydicom integration. | [PR #129](https://github.com/pydicom/pylibjpeg-openjpeg/pull/129) |
| [pylibjpeg-rle](https://github.com/pydicom/pylibjpeg-rle) | Native Linux ARM64 CI for the RLE codec. | [PR #62](https://github.com/pydicom/pylibjpeg-rle/pull/62) |
| [PyMedPhys](https://github.com/pymedphys/pymedphys) | TRF archive checksum enforcement under optimized Python. | [PR #2394](https://github.com/pymedphys/pymedphys/pull/2394) |
| [pynetdicom](https://github.com/pydicom/pynetdicom) | Password redaction in standard DICOM association logs. | [PR #1099](https://github.com/pydicom/pynetdicom/pull/1099) |
| [pynrrd](https://github.com/mhe/pynrrd) | Validation of nonpositive NRRD dimensions before data access. | [PR #173](https://github.com/mhe/pynrrd/pull/173) |
| [PyRadiomics](https://github.com/AIM-Harvard/pyradiomics) | HTTPS installation instructions, localhost-bound notebook examples, external-tool failure propagation in the experimental DICOM script, and download cache integrity. | [PR #956](https://github.com/AIM-Harvard/pyradiomics/pull/956) · [PR #957](https://github.com/AIM-Harvard/pyradiomics/pull/957) · [PR #958](https://github.com/AIM-Harvard/pyradiomics/pull/958) · [PR #959](https://github.com/AIM-Harvard/pyradiomics/pull/959) |
| [PyVista](https://github.com/pyvista/pyvista) | A multi-renderer example for actor cleanup. | [PR #9432](https://github.com/pyvista/pyvista/pull/9432) |
| [PyXNAT](https://github.com/pyxnat/pyxnat) | Restricted saved credential-file permissions on POSIX. | [PR #218](https://github.com/pyxnat/pyxnat/pull/218) |
| [RustSec / cargo-audit](https://github.com/rustsec/rustsec) | Documentation for target-platform value discovery. | [PR #1726](https://github.com/rustsec/rustsec/pull/1726) |
| [scikit-image](https://github.com/scikit-image/scikit-image) | Native Linux ARM64 build and test coverage. | [PR #8359](https://github.com/scikit-image/scikit-image/pull/8359) |
| [Semgrep](https://github.com/semgrep/semgrep) | Scope registration for untyped object-destructured parameters. | [PR #11991](https://github.com/semgrep/semgrep/pull/11991) |
| [Semgrep Rules](https://github.com/semgrep/semgrep-rules) | C# authorization-rule false-positive corrections, Terraform S3 versioning detection and guidance, and proposed retirement of a duplicate browser rule. | [PR #4085](https://github.com/semgrep/semgrep-rules/pull/4085) · [PR #4087](https://github.com/semgrep/semgrep-rules/pull/4087) · [PR #4096](https://github.com/semgrep/semgrep-rules/pull/4096) · [PR #4097](https://github.com/semgrep/semgrep-rules/pull/4097) |
| [silx](https://github.com/silx-kit/silx) | Native Linux ARM64 test coverage. | [PR #4742](https://github.com/silx-kit/silx/pull/4742) |
| [surfa](https://github.com/freesurfer/surfa) | Literal FreeView subtitle arguments. | [PR #86](https://github.com/freesurfer/surfa/pull/86) |
| [Syft](https://github.com/anchore/syft) | Alpine upstream URL references in CycloneDX SBOMs and parsed CPE attributes in custom output templates. | [PR #5437](https://github.com/anchore/syft/pull/5437) · [PR #5438](https://github.com/anchore/syft/pull/5438) |
| [TorchIO](https://github.com/TorchIO-project/torchio) | Preservation of HTTPS when dataset downloads fail. | [PR #1529](https://github.com/TorchIO-project/torchio/pull/1529) |
| [TotalSegmentator](https://github.com/wasserth/TotalSegmentator) | NORA mask-tagging arguments without shell interpretation. | [PR #627](https://github.com/wasserth/TotalSegmentator/pull/627) |
| [TractSeg](https://github.com/MIC-DKFZ/TractSeg) | Literal cleanup filenames. | [PR #294](https://github.com/MIC-DKFZ/TractSeg/pull/294) |
| [WORC](https://github.com/MStarmans91/WORC) | Literal parsing of PyRadiomics center-of-mass coordinates. | [PR #100](https://github.com/MStarmans91/WORC/pull/100) |
| [XCP-D](https://github.com/PennLINC/xcp_d) | Bounded buffering for example downloads; fork-PR lockfile validation with read-only permissions and a separate same-repository update job. | [PR #1638](https://github.com/PennLINC/xcp_d/pull/1638) · [PR #1640](https://github.com/PennLINC/xcp_d/pull/1640) |
| [xnatutils](https://github.com/Australian-Imaging-Service/xnatutils) | Containment of per-file XNAT download destinations. | [PR #16](https://github.com/Australian-Imaging-Service/xnatutils/pull/16) |
| [Zarr-Python](https://github.com/zarr-developers/zarr-python) | Native Linux ARM64 test coverage for Zarr. | [PR #4525](https://github.com/zarr-developers/zarr-python/pull/4525) |
| [zarrs-python](https://github.com/zarrs/zarrs-python) | Native Linux ARM64 CI for Python/Rust integration, including both test suites and type-stub checks. | [PR #199](https://github.com/zarrs/zarrs-python/pull/199) |

## Work incorporated by maintainers

These maintainer-authored follow-ups incorporated work from my original proposals, which were closed without merge.

| Project | Incorporated work | Original proposal and upstream follow-up |
| --- | --- | --- |
| [PaperBanana](https://github.com/dwzhu-pku/PaperBanana) | Critic-round controls and local/Ollama text routing, adapted from selected portions of my proposals. | [My PR #73](https://github.com/dwzhu-pku/PaperBanana/pull/73) → [Merged PR #95](https://github.com/dwzhu-pku/PaperBanana/pull/95); [my PR #74](https://github.com/dwzhu-pku/PaperBanana/pull/74) → [merged PR #96](https://github.com/dwzhu-pku/PaperBanana/pull/96) |
| [TorchXRayVision](https://github.com/mlmed/torchxrayvision) | Download-resilience work incorporated with attribution to my original proposal. | [My PR #199](https://github.com/mlmed/torchxrayvision/pull/199) → [Merged PR #200](https://github.com/mlmed/torchxrayvision/pull/200) |

## Public issue reports

| Project | Scope of work | Record |
| --- | --- | --- |
| [Codex](https://github.com/openai/codex) | Reported spurious unknown-conversation errors after successful ephemeral title generation. | [Issue #46289](https://github.com/openai/codex/issues/46289) · Open issue |
| [Gitleaks](https://github.com/gitleaks/gitleaks) | Reported deletion of an existing report before an invalid output format is rejected. | [Issue #2304](https://github.com/gitleaks/gitleaks/issues/2304) · Open issue |

## Work published in forks

These records document work in my forks. Upstream acceptance is separate.

| Project | Scope of work | Record |
| --- | --- | --- |
| [MRtrix3](https://github.com/MRtrix3/mrtrix3) | Fork patch passing build-error log paths directly to the pager. | [Commit 27b713f](https://github.com/jdotc1/mrtrix3/commit/27b713f264a7416762110f38364610e076344f07) · Published in fork |
| [NiftyNet](https://github.com/jdotc1/NiftyNet) | Fork proposal for TAR destination and member-type validation. | [PR #1](https://github.com/jdotc1/NiftyNet/pull/1) · Open in fork |

## Closed proposals

These proposals were closed without merge.

| Project | Scope of work | Record |
| --- | --- | --- |
| [Nilearn](https://github.com/nilearn/nilearn) | Proposed reuse of fitted NiftiMasker test setup. | [PR #6665](https://github.com/nilearn/nilearn/pull/6665) |
| [PaperBanana](https://github.com/dwzhu-pku/PaperBanana) | Proposed removal of hosted credential-editing controls. | [PR #70](https://github.com/dwzhu-pku/PaperBanana/pull/70) |
| [PaperOrchestra](https://github.com/Ar9av/PaperOrchestra) | Proposed native launcher integration with local acceptance checks. | [PR #12](https://github.com/Ar9av/PaperOrchestra/pull/12) · Closed draft |
| [pyvips](https://github.com/libvips/pyvips) | Native Linux ARM64 CI for libvips/CFFI integration. | [PR #1427](https://github.com/libvips/pyvips/pull/1427) |
| [TorchXRayVision](https://github.com/mlmed/torchxrayvision) | Preservation of existing downloads when transfers fail. | [PR #199](https://github.com/mlmed/torchxrayvision/pull/199) |

## Private reporting

[SimpleITK](https://github.com/SimpleITK/SimpleITK) — Private security disclosure. Details are not published here.
