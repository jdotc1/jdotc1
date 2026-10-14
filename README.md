### About me

Physician-scientist and independent developer working on medical imaging and scientific software for Apple silicon and native macOS, with a focus on MR-based radiomics.

I modernize existing tools and build utilities for DICOM, data processing, and research automation, with particular attention to numerical consistency, reliable data handling, and compatibility. I also use binary analysis and reverse engineering to understand application behavior. I’m sharing these tools on GitHub as they become ready for release.

### 🛡️ Open-source contributions

Security hardening and build reliability for medical imaging software.

- [3D Slicer](https://github.com/Slicer/Slicer) — macOS signing enforcement and dependency-boundary hardening.
- [ANTsPy](https://github.com/ANTsX/ANTsPy) — Cache integrity through HTTP failure rejection.
- [BIDScoin](https://github.com/Donders-Institute/bidscoin) — Shell interpretation prevention in SynthStrip arguments.
- [BrainIAK](https://github.com/brainiak/brainiak) — Literal-only parsing to prevent expression execution.
- [BrainStat](https://github.com/MICA-MNI/BrainStat) — Protection against caching incomplete downloads.
- [Clinica](https://github.com/aramis-lab/clinica) — Shell interpretation prevention for atlas paths.
- [dcm2niix](https://github.com/rordenlab/dcm2niix) — Dependency source pinning and controlled build configuration.
- [dcmqi](https://github.com/QIICR/dcmqi) — Reliable macOS SDK selection.
- [dcmstack](https://github.com/moloney/dcmstack) — Isolation of shared metadata-filter defaults.
- [deep-mr](https://github.com/INFN-MRI/deep-mr) — Defensive rejection of unsupported GPU devices.
- [deid](https://github.com/pydicom/deid) — Owner-only permissions for pixel-cleaner outputs.
- [dicom-numpy](https://github.com/innolitics/dicom-numpy) — Streamed DICOM extraction to reduce memory pressure.
- [dicom-validator](https://github.com/pydicom/dicom-validator) — HTML injection prevention through filename escaping.
- [dicomweb-client](https://github.com/ImagingDataCommons/dicomweb-client) — Path traversal prevention for DICOM output writes.
- [DIPY](https://github.com/dipy/dipy) — Integrity-check compatibility in restricted Python runtimes.
- [DLTK](https://github.com/DLTK/DLTK) — TAR path containment and unsafe-member rejection.
- [FAE](https://github.com/salan668/FAE) — Shell interpretation prevention when opening folders.
- [FastSurfer](https://github.com/Deep-MI/FastSurfer) — Shell interpretation prevention for link paths.
- [FreeSurfer](https://github.com/freesurfer/freesurfer) — Shell-free execution of SynthStrip containers.
- [HD-BET](https://github.com/MIC-DKFZ/HD-BET) — Isolated private staging for checkpoint downloads.
- [HeuDiConv](https://github.com/nipy/heudiconv) — Expression execution prevention in cached-table parsing.
- [highdicom](https://github.com/ImagingDataCommons/highdicom) — Malformed-fragment rejection before oversized reads.
- [ITK](https://github.com/InsightSoftwareConsortium/ITK) — Architecture-aware FFTW build configuration.
- [ITK-SNAP](https://github.com/pyushkevich/itksnap) — Shell interpretation prevention for launcher paths.
- [medicaldetectiontoolkit](https://github.com/MIC-DKFZ/medicaldetectiontoolkit) — Shell interpretation prevention in checkpoint cleanup.
- [MedPy](https://github.com/loli/medpy) — Python-compatible Boost library selection.
- [MIRTK](https://github.com/BioMedIA/MIRTK) — Correct Apple Silicon MATLAB extension selection.
- [MONAI Label](https://github.com/Project-MONAI/MONAILabel) — Rejection of failed authentication-discovery responses.
- [MRIQC](https://github.com/nipreps/mriqc) — Credential-disclosure reporting for download diagnostics.
- [MRtrix3](https://github.com/MRtrix3/mrtrix3) — Proposed shell-free build-error pager invocation.
- [netneurotools](https://github.com/netneurolab/netneurotools) — Explicit safety filtering for TAR extraction.
- [neuromaps](https://github.com/netneurolab/neuromaps) — Shell interpretation prevention in Workbench paths.
- [NiBabel](https://github.com/nipy/nibabel) — Malformed-input rejection before NIfTI payload reads.
- [NIFTI-Reader-JS](https://github.com/rii-mango/NIFTI-Reader-JS) — Negative extension-size rejection before payload access.
- [NiftyNet](https://github.com/jdotc1/NiftyNet) — Fork-based TAR path and member-type hardening.
- [NiftyReg](https://github.com/KCL-BMEIS/niftyreg) — ARM64-compatible SIMD build selection.
- [NiftySeg](https://github.com/KCL-BMEIS/NiftySeg) — Explicit target architectures in dependency builds.
- [Nilearn](https://github.com/nilearn/nilearn) — Archive extraction containment against path traversal.
- [Nipype](https://github.com/nipy/nipype) — Shell interpretation prevention in dependency inspection.
- [NiReports](https://github.com/nipreps/nireports) — End-of-input guards against unbounded SVG scanning.
- [NiWorkflows](https://github.com/nipreps/niworkflows) — Shell interpretation prevention in mri_info filenames.
- [nnU-Net](https://github.com/MIC-DKFZ/nnUNet) — Isolated private staging for model downloads.
- [PlatiPy](https://github.com/pyplati/platipy) — API credential protection, log access controls, and file containment.
- [pydicom](https://github.com/pydicom/pydicom) — Download-cache protection against HTTP error content.
- [PyMedPhys](https://github.com/pymedphys/pymedphys) — Checksum enforcement under optimized Python.
- [pynetdicom](https://github.com/pydicom/pynetdicom) — Credential exposure prevention in association logs.
- [pynrrd](https://github.com/mhe/pynrrd) — Malformed dimension rejection before NRRD data access.
- [pyplastimatch](https://github.com/ImagingDataCommons/pyplastimatch) — Failure propagation for conversion and resampling commands.
- [PyRadiomics](https://github.com/AIM-Harvard/pyradiomics) — Restricted notebook exposure and download-failure handling.
- [PyXNAT](https://github.com/pyxnat/pyxnat) — Credential-file protection with owner-only permissions.
- [RSNA Anonymizer](https://github.com/RSNA/anonymizer) — Per-process isolation of documentation helper caches.
- [SimpleITK](https://github.com/SimpleITK/SimpleITK) — Private vulnerability reporting and proposed archive hardening.
- [surfa](https://github.com/freesurfer/surfa) — Shell interpretation prevention in FreeView subtitles.
- [TorchIO](https://github.com/TorchIO-project/torchio) — Prevention of HTTPS-to-HTTP download downgrades.
- [TotalSegmentator](https://github.com/wasserth/TotalSegmentator) — Shell interpretation prevention in mask-tagging commands.
- [TractSeg](https://github.com/MIC-DKFZ/TractSeg) — Shell interpretation prevention in cleanup filenames.
- [XCP-D](https://github.com/PennLINC/xcp_d) — Bounded-buffer downloads to limit memory pressure.
- [xnatutils](https://github.com/Australian-Imaging-Service/xnatutils) — Path containment for XNAT file downloads.
