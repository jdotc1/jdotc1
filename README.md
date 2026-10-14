### About me

Physician-scientist and independent developer working on medical imaging and scientific software for Apple silicon and native macOS, with a focus on MR-based radiomics.

I modernize existing tools and build utilities for DICOM, data processing, and research automation, with particular attention to numerical consistency, reliable data handling, and compatibility. I also use binary analysis and reverse engineering to understand application behavior. I’m sharing these tools on GitHub as they become ready for release.

### 🛡️ Open-source contributions

Security hardening and build reliability for medical imaging software.

- [3D Slicer](https://github.com/Slicer/Slicer) — Stricter macOS signing, binary inspection, and dependency boundaries.
- [ANTsPy](https://github.com/ANTsX/ANTsPy) — Reject HTTP failures before they enter the data cache.
- [BIDScoin](https://github.com/Donders-Institute/bidscoin) — Protect SynthStrip command arguments from shell interpretation.
- [BrainIAK](https://github.com/brainiak/brainiak) — Replace executable expression parsing with literal-only parsing.
- [BrainStat](https://github.com/MICA-MNI/BrainStat) — Publish cached downloads only after successful transfer.
- [Clinica](https://github.com/aramis-lab/clinica) — Pass FreeSurfer atlas paths without shell interpretation.
- [dcm2niix](https://github.com/rordenlab/dcm2niix) — Pin dependency sources and preserve explicit build controls.
- [dcmqi](https://github.com/QIICR/dcmqi) — Honor macOS SDK names in build configuration.
- [dcmstack](https://github.com/moloney/dcmstack) — Isolate metadata-filter defaults from per-call changes.
- [deep-mr](https://github.com/INFN-MRI/deep-mr) — Reject unsupported device paths before CUDA conversion.
- [deid](https://github.com/pydicom/deid) — Restrict pixel-cleaner output directories to owner-only access.
- [dicom-numpy](https://github.com/innolitics/dicom-numpy) — Stream ZIP members to reduce decompression memory pressure.
- [dicom-validator](https://github.com/pydicom/dicom-validator) — Escape untrusted filenames in HTML reports.
- [dicomweb-client](https://github.com/ImagingDataCommons/dicomweb-client) — Prevent UID-derived writes outside the output directory.
- [DIPY](https://github.com/dipy/dipy) — Preserve integrity checks in security-restricted Python runtimes.
- [DLTK](https://github.com/DLTK/DLTK) — Reject unsafe TAR paths and non-file archive members.
- [FAE](https://github.com/salan668/FAE) — Remove shell interpretation from output-folder opening.
- [FastSurfer](https://github.com/Deep-MI/FastSurfer) — Protect FreeSurfer link paths from shell interpretation.
- [FreeSurfer](https://github.com/freesurfer/freesurfer) — Run SynthStrip Docker commands without a shell.
- [HD-BET](https://github.com/MIC-DKFZ/HD-BET) — Use private staging directories for checkpoint downloads.
- [HeuDiConv](https://github.com/nipy/heudiconv) — Parse cached tables without executing expressions.
- [highdicom](https://github.com/ImagingDataCommons/highdicom) — Reject malformed fragment lengths before oversized reads.
- [ITK](https://github.com/InsightSoftwareConsortium/ITK) — Honor target architecture when selecting FFTW SIMD defaults.
- [ITK-SNAP](https://github.com/pyushkevich/itksnap) — Protect macOS launcher paths with shell quoting.
- [MedPy](https://github.com/loli/medpy) — Select Python-compatible Boost libraries on macOS.
- [MIRTK](https://github.com/BioMedIA/MIRTK) — Correct native Apple Silicon MATLAB extension selection.
- [MONAI Label](https://github.com/Project-MONAI/MONAILabel) — Reject failed OpenID discovery responses before caching.
- [MRIQC](https://github.com/nipreps/mriqc) — Report credential disclosure in download error diagnostics.
- [MRtrix3](https://github.com/MRtrix3/mrtrix3) — Remove shell interpretation from build-error pager invocation.
- [neuromaps](https://github.com/netneurolab/neuromaps) — Preserve literal paths in Workbench command execution.
- [NiBabel](https://github.com/nipy/nibabel) — Validate NIfTI extension lengths before payload access.
- [NIFTI-Reader-JS](https://github.com/rii-mango/NIFTI-Reader-JS) — Reject negative extension sizes before payload access.
- [NiftyNet](https://github.com/jdotc1/NiftyNet) — Fork patch rejecting escaping TAR paths, links, and special files.
- [NiftyReg](https://github.com/KCL-BMEIS/niftyreg) — Prevent incompatible SSE selection for macOS ARM64 targets.
- [NiftySeg](https://github.com/KCL-BMEIS/NiftySeg) — Preserve target architectures in dependency builds.
- [Nilearn](https://github.com/nilearn/nilearn) — Enforce archive extraction destination boundaries.
- [Nipype](https://github.com/nipy/nipype) — Inspect executable dependencies without shell interpretation.
- [NiWorkflows](https://github.com/nipreps/niworkflows) — Pass mri_info filenames without shell interpretation.
- [nnU-Net](https://github.com/MIC-DKFZ/nnUNet) — Use private staging directories for model downloads.
- [PlatiPy](https://github.com/pyplati/platipy) — Protect API credentials, restrict log access, and contain file writes.
- [pydicom](https://github.com/pydicom/pydicom) — Reject HTTP error responses before saving downloads.
- [PyMedPhys](https://github.com/pymedphys/pymedphys) — Keep archive checksum guards active under Python optimization.
- [pynetdicom](https://github.com/pydicom/pynetdicom) — Redact authentication passwords from association logs.
- [PyRadiomics](https://github.com/AIM-Harvard/pyradiomics) — Restrict notebook exposure and reject failed tool or download results.
- [PyXNAT](https://github.com/pyxnat/pyxnat) — Restrict stored credential files to owner-only access.
- [SimpleITK](https://github.com/SimpleITK/SimpleITK) — Private vulnerability reporting with proposed archive hardening.
- [TorchIO](https://github.com/TorchIO-project/torchio) — Prevent silent HTTPS-to-HTTP download downgrades.
- [TotalSegmentator](https://github.com/wasserth/TotalSegmentator) — Remove shell interpretation from NORA mask tagging.
- [TractSeg](https://github.com/MIC-DKFZ/TractSeg) — Pass cleanup filenames as literal command arguments.
