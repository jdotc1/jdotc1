### About me

Physician-scientist, radiation oncologist, and independent developer focused on defensive security and privacy in medical-imaging and scientific software.

My open-source contributions span more than 50 repositories, covering security hardening, data integrity, and build reliability. My security work addresses credential and API-key exposure, missing access controls, unsafe command execution and data parsing, path traversal, archive extraction, and malformed-input handling. I also strengthen download integrity, dependency controls, and native macOS packaging.

I trace how software handles untrusted input and sensitive data, develop targeted fixes, and use synthetic regression tests to verify behavior. I document compatibility changes and validation limits, with particular attention to preserving scientific results and intended application behavior. My contributions include merged fixes, proposals under upstream review, and security reports.

I also build security and privacy tools: EntitlementDiff for comparing embedded macOS app entitlements between builds; DICOM Anonymizer for local metadata pseudonymization; and MacScope, a private binary-analysis and reverse-engineering workbench. My clinical and MR-based radiomics research informs this focus on protecting sensitive imaging workflows while modernizing the software they depend on.

### Selected security contributions

Selected work in security analysis, credential protection, and safer medical-imaging software. Open pull requests are proposed changes, distinct from merged contributions and published tools.

**[Semgrep — authorization-rule precision](https://github.com/semgrep/semgrep-rules/pull/4085) · PR #4085 · Open**

Proposed a targeted correction to a C# authorization rule that flags controllers with explicit authentication schemes. Added 14 regression and control cases while preserving the existing rule scope and positive detections. The PR documents before-and-after engine results and full local repository validation.

**[pynetdicom — credential protection](https://github.com/pydicom/pynetdicom/pull/1099) · PR #1099 · Open**

Proposed password redaction in standard sent and received DICOM association logs, with regression tests checking both returned messages and captured logging output. The change is scoped to standard association logging.

**[PlatiPy — API-key handling](https://github.com/pyplati/platipy/pull/322) · PR #322 · Open**

Proposed consistent protection for a custom API-key header across HTTP redirect authentication boundaries, covering all 12 authenticated client request sites. The PR documents synthetic checks for same-origin retention and removal across host, port, and HTTPS-downgrade boundaries.

**[BIDScoin — command and path handling](https://github.com/Donders-Institute/bidscoin/pull/302) · PR #302 · Merged**

Hardened local SynthStrip command construction so image paths containing spaces and shell metacharacters remain literal arguments. Added a focused regression test; the contribution was accepted and merged upstream.

**[EntitlementDiff — original security-review tooling](https://github.com/jdotc1/EntitlementDiff/releases/tag/v0.1.2) · v0.1.2 · Published**

Built a native macOS tool for reviewing changes in embedded entitlement declarations between application builds without launching the inspected applications. Published source and an Apple-silicon application, with explicit distinctions between declared entitlements, effective permissions, and signature verification.

### 🛡️ Open-source contributions

Security hardening, analysis tooling, data integrity, and build reliability across medical-imaging and scientific software.

- [3D Slicer](https://github.com/Slicer/Slicer) — Signing failure enforcement and macOS dependency escape prevention.
- [ANTsPy](https://github.com/ANTsX/ANTsPy) — Reject HTTP error content before cache publication.
- [BIDScoin](https://github.com/Donders-Institute/bidscoin) — Command-injection hardening through literal SynthStrip arguments.
- [BrainIAK](https://github.com/brainiak/brainiak) — Remove expression execution from noise-dictionary parsing.
- [BrainStat](https://github.com/MICA-MNI/BrainStat) — Prevent partial downloads from becoming trusted cache entries.
- [Clinica](https://github.com/aramis-lab/clinica) — Command-injection hardening for FreeSurfer atlas paths.
- [dcm2niix](https://github.com/rordenlab/dcm2niix) — Dependency source pinning and explicit toolchain controls.
- [dcmjs](https://github.com/dcmjs-org/dcmjs) — Validate byte counts before binary data reads.
- [dcmqi](https://github.com/QIICR/dcmqi) — Reliable macOS SDK selection.
- [dcmstack](https://github.com/moloney/dcmstack) — Prevent cross-call mutation of metadata-filter policy.
- [deep-mr](https://github.com/INFN-MRI/deep-mr) — Defensive rejection of unsupported GPU devices.
- [deid](https://github.com/pydicom/deid) — Restrict local access to pixel-cleaner outputs.
- [dicom-numpy](https://github.com/innolitics/dicom-numpy) — Limit decompression memory use with streamed ZIP reads.
- [dicom-validator](https://github.com/pydicom/dicom-validator) — Prevent filename-based HTML injection in reports.
- [dicomParser](https://github.com/cornerstonejs/dicomParser) — Reject invalid and out-of-bounds binary stream seeks.
- [dicomweb-client](https://github.com/ImagingDataCommons/dicomweb-client) — Block path traversal in UID-derived output filenames.
- [DIPY](https://github.com/dipy/dipy) — Retain dataset integrity checks in restricted runtimes.
- [DLTK](https://github.com/DLTK/DLTK) — Block archive path escapes and unsafe TAR member types.
- [FAE](https://github.com/salan668/FAE) — Remove shell execution from folder-opening commands.
- [FastSurfer](https://github.com/Deep-MI/FastSurfer) — Command-injection hardening for filesystem link arguments.
- [FreeSurfer](https://github.com/freesurfer/freesurfer) — Remove shell execution from SynthStrip Docker commands.
- [Gitleaks](https://github.com/gitleaks/gitleaks) — Report destructive report-file validation that can erase existing security reports.
- [HD-BET](https://github.com/MIC-DKFZ/HD-BET) — Isolate checkpoint downloads in private temporary directories.
- [HeuDiConv](https://github.com/nipy/heudiconv) — Eliminate executable expression parsing from cached tables.
- [highdicom](https://github.com/ImagingDataCommons/highdicom) — Reject malformed lengths before excessive payload reads.
- [InVesalius](https://github.com/invesalius/invesalius3) — Restore TLS verification and bound update-discovery requests.
- [ITK](https://github.com/InsightSoftwareConsortium/ITK) — Architecture-aware FFTW build configuration.
- [ITK-SNAP](https://github.com/pyushkevich/itksnap) — Command-injection hardening for macOS launcher paths.
- [medicaldetectiontoolkit](https://github.com/MIC-DKFZ/medicaldetectiontoolkit) — Prevent shell interpretation of checkpoint cleanup paths.
- [MedPy](https://github.com/loli/medpy) — Python-compatible Boost library selection.
- [minc-toolkit-v2](https://github.com/BIC-MNI/minc-toolkit-v2) — Preserve explicit macOS build settings in HDF5 dependencies.
- [MIRTK](https://github.com/BioMedIA/MIRTK) — Correct Apple Silicon MATLAB extension selection.
- [MONAI](https://github.com/Project-MONAI/MONAI) — Propagate download publication failures instead of masking errors.
- [MONAI Label](https://github.com/Project-MONAI/MONAILabel) — Reject failed identity-provider discovery before cache reuse.
- [MRIQC](https://github.com/nipreps/mriqc) — Report authentication-credential leakage in error diagnostics.
- [MRtrix3](https://github.com/MRtrix3/mrtrix3) — Proposed removal of shell execution from error-log paging.
- [netneurotools](https://github.com/netneurolab/netneurotools) — Apply safe extraction filters to downloaded TAR archives.
- [neuromaps](https://github.com/netneurolab/neuromaps) — Command-injection hardening for Workbench path arguments.
- [NiBabel](https://github.com/nipy/nibabel) — Reject malformed NIfTI lengths before payload processing.
- [NIFTI-Reader-JS](https://github.com/rii-mango/NIFTI-Reader-JS) — Reject negative NIfTI lengths before payload processing.
- [NiftyNet](https://github.com/jdotc1/NiftyNet) — Fork patch blocking TAR path escapes, links, and special files.
- [NiftyReg](https://github.com/KCL-BMEIS/niftyreg) — ARM64-compatible SIMD build selection.
- [NiftySeg](https://github.com/KCL-BMEIS/NiftySeg) — Explicit target architectures in dependency builds.
- [Nilearn](https://github.com/nilearn/nilearn) — Block archive traversal using destination containment checks.
- [NiPy](https://github.com/nipy/nipy) — Remove intermediate shell execution from MATLAB launch.
- [Nipype](https://github.com/nipy/nipype) — Remove shell execution from executable dependency inspection.
- [NiReports](https://github.com/nipreps/nireports) — Prevent unterminated SVG input from causing endless scanning.
- [nitrain](https://github.com/nitrain/nitrain) — Block OpenNeuro download paths outside the data root.
- [NiWorkflows](https://github.com/nipreps/niworkflows) — Remove shell execution from mri_info filename handling.
- [nnU-Net](https://github.com/MIC-DKFZ/nnUNet) — Isolate model downloads in private staging directories.
- [Papaya](https://github.com/rii-mango/Papaya) — Prevent HTML interpretation of image title labels.
- [PlatiPy](https://github.com/pyplati/platipy) — Prevent credential leakage, unauthorized log access, and file path escapes.
- [pydicom](https://github.com/pydicom/pydicom) — Reject HTTP error bodies before writing cached data.
- [PyMedPhys](https://github.com/pymedphys/pymedphys) — Prevent optimized Python from disabling checksum enforcement.
- [pynetdicom](https://github.com/pydicom/pynetdicom) — Prevent authentication-password leakage through logs.
- [pynrrd](https://github.com/mhe/pynrrd) — Reject invalid NRRD dimensions before data processing.
- [pyplastimatch](https://github.com/ImagingDataCommons/pyplastimatch) — Stop failed external processes from appearing successful.
- [PyRadiomics](https://github.com/AIM-Harvard/pyradiomics) — Reduce notebook network exposure and reject failed downloads.
- [PyXNAT](https://github.com/pyxnat/pyxnat) — Prevent other local users from reading credential files.
- [RSNA Anonymizer](https://github.com/RSNA/anonymizer) — Isolate helper caches to reduce shared temporary-file risks.
- [Semgrep Rules (PR #4085)](https://github.com/semgrep/semgrep-rules/pull/4085) — Proposed authorization-rule precision fix for explicit authentication schemes (open).
- [SimpleITK](https://github.com/SimpleITK/SimpleITK) — Private security disclosure and proposed safe archive extraction.
- [surfa](https://github.com/freesurfer/surfa) — Command-injection hardening for FreeView subtitle arguments.
- [TorchIO](https://github.com/TorchIO-project/torchio) — Block insecure HTTP fallback after HTTPS failures.
- [TorchXRayVision](https://github.com/mlmed/torchxrayvision) — Protect existing downloads from failed transfer replacement.
- [TotalSegmentator](https://github.com/wasserth/TotalSegmentator) — Remove shell execution from NORA mask-tagging commands.
- [TractSeg](https://github.com/MIC-DKFZ/TractSeg) — Prevent shell interpretation of cleanup filenames.
- [WORC](https://github.com/MStarmans91/WORC) — Remove expression execution from coordinate parsing.
- [XCP-D](https://github.com/PennLINC/xcp_d) — Bound download buffering to reduce memory-exhaustion risk.
- [xnatutils](https://github.com/Australian-Imaging-Service/xnatutils) — Block download destinations outside the selected directory.
