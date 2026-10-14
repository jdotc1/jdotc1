### About me

Physician-scientist and independent developer building medical imaging, scientific, and security-focused software for Apple silicon and native macOS, with a research focus on MR-based radiomics.

I build local tools for DICOM processing, MRI metadata comparison, scientific automation, and application inspection, with particular attention to numerical consistency, reliable data handling, and security. My public projects include:

- [dicom-anonymizer](https://github.com/jdotc1/dicom-anonymizer) — Local DICOM metadata pseudonymization with a Python engine and native macOS source.
- [EntitlementDiff](https://github.com/jdotc1/EntitlementDiff) — Native macOS comparison of embedded app entitlements between builds, with explicit architecture selection.
- [prism-native-mcp](https://github.com/jdotc1/prism-native-mcp) — Local MCP integration for native GraphPad Prism tables, analyses, graphs, and layouts.
- [SidecarCompare](https://github.com/jdotc1/SidecarCompare) — Native macOS comparison of MRI JSON sidecars with exact decimal handling and read-only local snapshots.

I also modernize and port existing applications to ARM64 and Apple silicon, improving native macOS compatibility, performance, and build reliability.

### 🛡️ Open-source contributions

Security hardening and build reliability for medical imaging software.

- [3D Slicer](https://github.com/Slicer/Slicer) — Signing failure enforcement and macOS dependency escape prevention.
- [ANTsPy](https://github.com/ANTsX/ANTsPy) — Reject HTTP error content before cache publication.
- [BIDScoin](https://github.com/Donders-Institute/bidscoin) — Command-injection hardening through literal SynthStrip arguments.
- [BrainIAK](https://github.com/brainiak/brainiak) — Remove expression execution from noise-dictionary parsing.
- [BrainStat](https://github.com/MICA-MNI/BrainStat) — Prevent partial downloads from becoming trusted cache entries.
- [Clinica](https://github.com/aramis-lab/clinica) — Command-injection hardening for FreeSurfer atlas paths.
- [dcm2niix](https://github.com/rordenlab/dcm2niix) — Dependency source pinning and explicit toolchain controls.
- [dcmqi](https://github.com/QIICR/dcmqi) — Reliable macOS SDK selection.
- [dcmstack](https://github.com/moloney/dcmstack) — Prevent cross-call mutation of metadata-filter policy.
- [deep-mr](https://github.com/INFN-MRI/deep-mr) — Defensive rejection of unsupported GPU devices.
- [deid](https://github.com/pydicom/deid) — Restrict local access to pixel-cleaner outputs.
- [dicom-numpy](https://github.com/innolitics/dicom-numpy) — Limit decompression memory use with streamed ZIP reads.
- [dicom-validator](https://github.com/pydicom/dicom-validator) — Prevent filename-based HTML injection in reports.
- [dicomweb-client](https://github.com/ImagingDataCommons/dicomweb-client) — Block path traversal in UID-derived output filenames.
- [DIPY](https://github.com/dipy/dipy) — Retain dataset integrity checks in restricted runtimes.
- [DLTK](https://github.com/DLTK/DLTK) — Block archive path escapes and unsafe TAR member types.
- [FAE](https://github.com/salan668/FAE) — Remove shell execution from folder-opening commands.
- [FastSurfer](https://github.com/Deep-MI/FastSurfer) — Command-injection hardening for filesystem link arguments.
- [FreeSurfer](https://github.com/freesurfer/freesurfer) — Remove shell execution from SynthStrip Docker commands.
- [HD-BET](https://github.com/MIC-DKFZ/HD-BET) — Isolate checkpoint downloads in private temporary directories.
- [HeuDiConv](https://github.com/nipy/heudiconv) — Eliminate executable expression parsing from cached tables.
- [highdicom](https://github.com/ImagingDataCommons/highdicom) — Reject malformed lengths before excessive payload reads.
- [ITK](https://github.com/InsightSoftwareConsortium/ITK) — Architecture-aware FFTW build configuration.
- [ITK-SNAP](https://github.com/pyushkevich/itksnap) — Command-injection hardening for macOS launcher paths.
- [medicaldetectiontoolkit](https://github.com/MIC-DKFZ/medicaldetectiontoolkit) — Prevent shell interpretation of checkpoint cleanup paths.
- [MedPy](https://github.com/loli/medpy) — Python-compatible Boost library selection.
- [MIRTK](https://github.com/BioMedIA/MIRTK) — Correct Apple Silicon MATLAB extension selection.
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
- [Nipype](https://github.com/nipy/nipype) — Remove shell execution from executable dependency inspection.
- [NiReports](https://github.com/nipreps/nireports) — Prevent unterminated SVG input from causing endless scanning.
- [NiWorkflows](https://github.com/nipreps/niworkflows) — Remove shell execution from mri_info filename handling.
- [nnU-Net](https://github.com/MIC-DKFZ/nnUNet) — Isolate model downloads in private staging directories.
- [PlatiPy](https://github.com/pyplati/platipy) — Prevent credential leakage, unauthorized log access, and file path escapes.
- [pydicom](https://github.com/pydicom/pydicom) — Reject HTTP error bodies before writing cached data.
- [PyMedPhys](https://github.com/pymedphys/pymedphys) — Prevent optimized Python from disabling checksum enforcement.
- [pynetdicom](https://github.com/pydicom/pynetdicom) — Prevent authentication-password leakage through logs.
- [pynrrd](https://github.com/mhe/pynrrd) — Reject invalid NRRD dimensions before data processing.
- [pyplastimatch](https://github.com/ImagingDataCommons/pyplastimatch) — Stop failed external processes from appearing successful.
- [PyRadiomics](https://github.com/AIM-Harvard/pyradiomics) — Reduce notebook network exposure and reject failed downloads.
- [PyXNAT](https://github.com/pyxnat/pyxnat) — Prevent other local users from reading credential files.
- [RSNA Anonymizer](https://github.com/RSNA/anonymizer) — Isolate helper caches to reduce shared temporary-file risks.
- [SimpleITK](https://github.com/SimpleITK/SimpleITK) — Private security disclosure and proposed safe archive extraction.
- [surfa](https://github.com/freesurfer/surfa) — Command-injection hardening for FreeView subtitle arguments.
- [TorchIO](https://github.com/TorchIO-project/torchio) — Block insecure HTTP fallback after HTTPS failures.
- [TotalSegmentator](https://github.com/wasserth/TotalSegmentator) — Remove shell execution from NORA mask-tagging commands.
- [TractSeg](https://github.com/MIC-DKFZ/TractSeg) — Prevent shell interpretation of cleanup filenames.
- [XCP-D](https://github.com/PennLINC/xcp_d) — Bound download buffering to reduce memory-exhaustion risk.
- [xnatutils](https://github.com/Australian-Imaging-Service/xnatutils) — Block download destinations outside the selected directory.
