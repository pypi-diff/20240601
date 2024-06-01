# Comparing `tmp/panpipelines-1.0.1.tar.gz` & `tmp/panpipelines-1.0.2.tar.gz`

## Comparing `panpipelines-1.0.1.tar` & `panpipelines-1.0.2.tar`

### file list

```diff
@@ -1,192 +1,204 @@
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-1.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/run_pan250.sh
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/res-01_atlas-Arterial_desc-level2_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_desc-level2_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0   159508 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_dseg.nii.gz
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_seg.json
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0    30469 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_dseg.nii.gz
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_seg.json
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/config/license.txt
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/config/pan250.config
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/config/pan250_eddyparams.json
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/config/pan250_eddyparams_cuda.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PAN250_Deployment/config/credentials/credentials.json
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/README.md
--rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/run_pan_slurm.sh
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/README.md
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/ArterialAtlasLabels.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HARVCORT/README.md
--rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HARVSUBCORT/README.md
--rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/README.md
--rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
--rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
--rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
--rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/JHU/JHU-labels_index.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/JHU/JHU-tracts_index.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/JHU/README.md
--rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
--rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/XTRACT_index.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
--rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/README.md
--rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/fs_default.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/hcpmmp1_subfields_atlas/README.md
--rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
--rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
--rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/eddy_params.json
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/eddy_params_cpu.json
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/freebash.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/license.txt
--rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/panpipeconfig_expanded_slurm.config
--rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/panpipeconfig_slurm.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.1/deployment/config/credentials/credentials.json
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-1.0.1/example/run_pan_example.sh
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-1.0.1/example/config/panpipeconfig_example.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.1/example/config/credentials/credentials_example.json
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/Factory.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/__init__.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/group_subjects.py
--rwxr-xr-x   0        0        0    18596 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pan_processing.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/single_subject.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/version.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/__init__.py
--rw-r--r--   0        0        0    22370 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/antstransform.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/aslprep.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/atlascreate.py
--rw-r--r--   0        0        0    33138 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/basil.py
--rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/collate_csv_group.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/collate_csv_single.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/dummy.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/fmriprep.py
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/freesurfer.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/fslanat.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/glm_randomize_group.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/lst.py
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/mriqc.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/noddi.py
--rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/parse_textdata.py
--rw-r--r--   0        0        0    27631 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/preproc.py
--rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/qsiprep.py
--rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/roi_extract.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/roi_mean_group.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/roi_mean_single.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/nodes/tensor.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/aslprep_panpipeline.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/basil_panpipeline.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/collatecsv_panpipeline.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/dummy_panpipeline.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/fmriprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/freesurfer_panpipeline.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/lst_panpipeline.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/mriqc_panpipeline.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/noddi_panpipeline.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/preproc_panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/qsiprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/roiextract_panpipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/tensor_panpipeline.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/textmeasures_panpipeline.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/pipelines/volmeasures_panpipeline.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/__init__.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/aslprep_panscript.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/fmriprep_panscript.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/mne_make_surfaces.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/pancontainer_panscript.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/panscript.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/scripts/sdcflows_fieldmap.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/utils/__init__.py
--rw-r--r--   0        0        0    32043 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/utils/transformer.py
--rw-r--r--   0        0        0    91503 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/utils/util_functions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/aslprep_workflow.py
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/basil_workflow.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/collatecsv_workflow.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/collatecsvgroup_workflow.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/dummy_workflow.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/fmriprep_workflow.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/freesurfer_workflow.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/lst_workflow.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/mriqc_workflow.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/noddi_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/preproc_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/qsiprep_workflow.py
--rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/roiextract_workflow.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/tensor_workflow.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/textmeasures_workflow.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-1.0.1/src/panpipelines/workflows/volmeasures_workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-1.0.1/tests/test_PANFactory.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-1.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-1.0.1/LICENSE
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-1.0.1/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/run_pan250.sh
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/res-01_atlas-Arterial_desc-level2_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_desc-level2_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0   159508 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_dseg.nii.gz
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_seg.json
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0    30469 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_dseg.nii.gz
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_seg.json
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/config/license.txt
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/config/pan250.config
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/config/pan250_eddyparams.json
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/config/pan250_eddyparams_cuda.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PAN250_Deployment/config/credentials/credentials.json
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/README.md
+-rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/run_pan_slurm.sh
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/README.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/ArterialAtlasLabels.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HARVCORT/README.md
+-rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HARVSUBCORT/README.md
+-rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/README.md
+-rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
+-rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
+-rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
+-rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/JHU/JHU-labels_index.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/JHU/JHU-tracts_index.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/JHU/README.md
+-rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
+-rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/XTRACT_index.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
+-rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/README.md
+-rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/fs_default.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/hcpmmp1_subfields_atlas/README.md
+-rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
+-rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
+-rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/eddy_params.json
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/eddy_params_cpu.json
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/freebash.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/license.txt
+-rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/panpipeconfig_expanded_slurm.config
+-rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/panpipeconfig_slurm.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.2/deployment/config/credentials/credentials.json
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-1.0.2/example/run_pan_example.sh
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-1.0.2/example/config/panpipeconfig_example.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.2/example/config/credentials/credentials_example.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/createTable.m
+-rw-r--r--   0        0        0    21046 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/enable_aslmetrics.m
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/enable_aslmetrics.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/glob.m
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/pantransformed_enable_aslmetrics.sh
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/validmean.m
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/validmedian.m
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.2/external_scripts/enable_aslmetrics/validvariance.m
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/Factory.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/__init__.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/group_subjects.py
+-rwxr-xr-x   0        0        0    18810 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pan_processing.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/single_subject.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/version.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/__init__.py
+-rw-r--r--   0        0        0    22370 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/antstransform.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/aslprep.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/atlascreate.py
+-rw-r--r--   0        0        0    33138 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/basil.py
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/collate_csv_group.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/collate_csv_single.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/dummy.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/fmriprep.py
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/freesurfer.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/fslanat.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/glm_randomize_group.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/lst.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/mriqc.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/noddi.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/pancontainergroup.py
+-rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/parse_textdata.py
+-rw-r--r--   0        0        0    27631 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/preproc.py
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/qsiprep.py
+-rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/roi_extract.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/roi_mean_group.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/roi_mean_single.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/nodes/tensor.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/aslprep_panpipeline.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/basil_panpipeline.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/collatecsv_panpipeline.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/dummy_panpipeline.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/fmriprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/freesurfer_panpipeline.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/lst_panpipeline.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/mriqc_panpipeline.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/noddi_panpipeline.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/pancontainergroup_panpipeline.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/preproc_panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/qsiprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/roiextract_panpipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/tensor_panpipeline.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/textmeasures_panpipeline.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/pipelines/volmeasures_panpipeline.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/aslprep_panscript.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/fmriprep_panscript.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/mne_make_surfaces.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/pancontainer_panscript.py
+-rw-r--r--   0        0        0    41573 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/paninfo_bidsqc.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/panscript.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/scripts/sdcflows_fieldmap.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/utils/__init__.py
+-rw-r--r--   0        0        0    32043 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/utils/transformer.py
+-rw-r--r--   0        0        0    93557 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/utils/util_functions.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/aslprep_workflow.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/basil_workflow.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/collatecsv_workflow.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/collatecsvgroup_workflow.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/dummy_workflow.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/fmriprep_workflow.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/freesurfer_workflow.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/lst_workflow.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/mriqc_workflow.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/noddi_workflow.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/pancontainergroup_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/preproc_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/qsiprep_workflow.py
+-rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/roiextract_workflow.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/tensor_workflow.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/textmeasures_workflow.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-1.0.2/src/panpipelines/workflows/volmeasures_workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-1.0.2/tests/test_PANFactory.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-1.0.2/LICENSE
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-1.0.2/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-1.0.2/PKG-INFO
```

### Comparing `panpipelines-1.0.1/.github/workflows/python-package.yml` & `panpipelines-1.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/.github/workflows/python-publish.yml` & `panpipelines-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/README.md` & `panpipelines-1.0.2/PAN250_Deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/run_pan250.sh` & `panpipelines-1.0.2/PAN250_Deployment/run_pan250.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/README.md` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_dseg.nii.gz` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_seg.json` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_desc-level2_seg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_dseg.nii.gz` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_seg.json` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_desc-level2_seg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.2/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/README.md` & `panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-1.0.2/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/batch_scripts/group_template.pbs` & `panpipelines-1.0.2/PAN250_Deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/batch_scripts/participant_template.pbs` & `panpipelines-1.0.2/PAN250_Deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PAN250_Deployment/config/pan250.config` & `panpipelines-1.0.2/PAN250_Deployment/config/pan250.config`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/README.md` & `panpipelines-1.0.2/deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/run_pan_slurm.sh` & `panpipelines-1.0.2/deployment/run_pan_slurm.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/AAL3v1_1mm_index.txt` & `panpipelines-1.0.2/deployment/atlas/AAL3/AAL3v1_1mm_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/README.md` & `panpipelines-1.0.2/deployment/atlas/AAL3/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv` & `panpipelines-1.0.2/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv` & `panpipelines-1.0.2/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py` & `panpipelines-1.0.2/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/Arterial/README.md` & `panpipelines-1.0.2/deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz` & `panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json` & `panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.2/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt` & `panpipelines-1.0.2/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz` & `panpipelines-1.0.2/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz` & `panpipelines-1.0.2/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/README.md` & `panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt` & `panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt` & `panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot` & `panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot` & `panpipelines-1.0.2/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/JHU/JHU-labels_index.txt` & `panpipelines-1.0.2/deployment/atlas/JHU/JHU-labels_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/JHU/JHU-tracts_index.txt` & `panpipelines-1.0.2/deployment/atlas/JHU/JHU-tracts_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz` & `panpipelines-1.0.2/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz` & `panpipelines-1.0.2/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/README.md` & `panpipelines-1.0.2/deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/XTRACT_index.txt` & `panpipelines-1.0.2/deployment/atlas/XTRACT/XTRACT_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt` & `panpipelines-1.0.2/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-1.0.2/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json` & `panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz` & `panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz` & `panpipelines-1.0.2/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt` & `panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/fs_a2009s.txt` & `panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/fs_a2009s.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/freesurfer_atlas/fs_default.txt` & `panpipelines-1.0.2/deployment/atlas/freesurfer_atlas/fs_default.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt` & `panpipelines-1.0.2/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt` & `panpipelines-1.0.2/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/batch_scripts/group_template.pbs` & `panpipelines-1.0.2/deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/batch_scripts/participant_template.pbs` & `panpipelines-1.0.2/deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/config/panpipeconfig_expanded_slurm.config` & `panpipelines-1.0.2/deployment/config/panpipeconfig_expanded_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/deployment/config/panpipeconfig_slurm.config` & `panpipelines-1.0.2/deployment/config/panpipeconfig_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/example/config/panpipeconfig_example.config` & `panpipelines-1.0.2/example/config/panpipeconfig_example.config`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/Factory.py` & `panpipelines-1.0.2/src/panpipelines/Factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,21 @@
                 scriptclass = getattr(module,name)
                 return scriptclass
             else:
                 return None
         except Exception as ex:
             pass
 
+    def get_runscript(self, name):
+        try:
+            module = __import__(f"{self.script_module}.{name}",fromlist=[name])
+            return module
+        except Exception as ex:
+            pass
+
     def get_processflow(self, name):
         if "script" in name:
             processflow = self.get_script(name)
         elif "pipeline" in name:
             processflow = self.get_pipeline(name)           
         elif "workflow" in name:
             processflow = self.get_workflow(name)
```

### Comparing `panpipelines-1.0.1/src/panpipelines/group_subjects.py` & `panpipelines-1.0.2/src/panpipelines/group_subjects.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pan_processing.py` & `panpipelines-1.0.2/src/panpipelines/pan_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,17 +216,22 @@
     runtime_labels = panpipe_labels.copy()
 
     for pipeline in pipelines:
         LOGGER.info(f"Processing pipeline : {pipeline}")
         panpipe_labels = updateParams(panpipe_labels, "PIPELINE", pipeline)
         panpipe_labels = process_labels(panpipeconfig_json,panpipeconfig_file,panpipe_labels,pipeline)
 
-        # rather rigid - but we foreshadow the worfflow directory here and use a param so it is useable
-        wf_dir = f"<PIPELINE_DIR>/{pipeline}/<PARTICIPANT_XNAT_PROJECT>/sub-<PARTICIPANT_LABEL>/ses-<PARTICIPANT_SESSION>/{pipeline}_wf"
-        panpipe_labels = updateParams(panpipe_labels,f"WORKFLOW_DIR",wf_dir)
+        analysis_level = getParams(panpipe_labels,"ANALYSIS_LEVEL")
+        if analysis_level == "group":
+            # rather rigid - but we foreshadow the worfflow directory here and use a param so it is useable
+            wf_dir = f"<PIPELINE_DIR>/{pipeline}/group/{pipeline}_wf"
+            panpipe_labels = updateParams(panpipe_labels,f"WORKFLOW_DIR",wf_dir)
+        else:
+            wf_dir = f"<PIPELINE_DIR>/{pipeline}/<PARTICIPANT_XNAT_PROJECT>/sub-<PARTICIPANT_LABEL>/ses-<PARTICIPANT_SESSION>/{pipeline}_wf"
+            panpipe_labels = updateParams(panpipe_labels,f"WORKFLOW_DIR",wf_dir)
 
         # We handle the <DEPENDENCY> key specially as this is a list that we need to resolve into DEPENDENCY1, DEPENDENCY2, ...DEPENDENCYN
         dependency_list = getParams(panpipe_labels,"DEPENDENCY")
         if dependency_list:
             depcount=1
             if isinstance(dependency_list,list):
                 for dependency in dependency_list:
@@ -241,16 +246,14 @@
                 panpipe_labels = updateParams(panpipe_labels,f"DEPENDENCY{depcount}_DIR",dependency_dir1)
                 dependency_dir = f"<PIPELINE_DIR>/<DEPENDENCY>/<PARTICIPANT_XNAT_PROJECT>/sub-<PARTICIPANT_LABEL>/ses-<PARTICIPANT_SESSION>/<DEPENDENCY>_wf"
                 panpipe_labels = updateParams(panpipe_labels,f"DEPENDENCY_DIR",dependency_dir)
             
         # Now we can resolve all the references based on precedence in the pipeline section
         panpipe_labels = update_labels(panpipe_labels)
 
-        analysis_level = getParams(panpipe_labels,"ANALYSIS_LEVEL")
-
         processing_environment=getParams(panpipe_labels,"PROCESSING_ENVIRONMENT") 
 
         if processing_environment is None  or processing_environment not in PROCESSING_OPTIONS:
             processing_environment = "slurm"
 
         if processing_environment == "slurm":
             analysis_node = getParams(panpipe_labels,"ANALYSIS_NODE")
```

### Comparing `panpipelines-1.0.1/src/panpipelines/single_subject.py` & `panpipelines-1.0.2/src/panpipelines/single_subject.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/antstransform.py` & `panpipelines-1.0.2/src/panpipelines/nodes/antstransform.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/aslprep.py` & `panpipelines-1.0.2/src/panpipelines/nodes/aslprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/atlascreate.py` & `panpipelines-1.0.2/src/panpipelines/nodes/atlascreate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/basil.py` & `panpipelines-1.0.2/src/panpipelines/nodes/basil.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/collate_csv_group.py` & `panpipelines-1.0.2/src/panpipelines/nodes/collate_csv_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,34 +90,58 @@
         collate_name_left = getParams(labels_dict,"COLLATE_NAME_LEFT")
         if not collate_name_left:
             if not pipeline:
                 collate_name_left="csvgroup"
             else:
                 collate_name_left="pipeline"
 
+        collate_prefix_left = getParams(labels_dict,"COLLATE_PREFIX_LEFT")
+
         roi_csv_inner_left = os.path.join(roi_output_dir,'{}_{}_inner_left.csv'.format("group",collate_name_left))
         roi_csv_outer_left = os.path.join(roi_output_dir,'{}_{}_outer_left.csv'.format("group",collate_name_left))
 
         #create sorted output
         cum_df_inner_left = cum_df_inner_left.reindex(sorted(cum_df_inner_left.columns), axis=1)
         if "session_id" in cum_df_inner_left.columns and "subject_id" in cum_df_inner_left.columns:
             sub_col = cum_df_inner_left.pop("subject_id")
             ses_col = cum_df_inner_left.pop("session_id")
 
+            if collate_prefix_left:
+                orig_cols = cum_df_inner_left.columns.tolist()
+                new_cols = [f"{collate_prefix_left}.{x}" for x in orig_cols]
+                new_dict = dict(zip(orig_cols,new_cols))
+                cum_df_inner_left = cum_df_inner_left.rename(columns=new_dict)
+
             cum_df_inner_left.insert(0,"session_id",ses_col)
             cum_df_inner_left.insert(0,"subject_id",sub_col)
+        elif collate_prefix_left:
+                orig_cols = cum_df_inner_left.columns.tolist()
+                new_cols = [f"{collate_prefix_left}.{x}" for x in orig_cols]
+                new_dict = dict(zip(orig_cols,new_cols))
+                cum_df_inner_left = cum_df_inner_left.rename(columns=new_dict)
 
         #create sorted output
         cum_df_outer_left = cum_df_outer_left.reindex(sorted(cum_df_outer_left.columns), axis=1)
         if "session_id" in cum_df_outer_left.columns and "subject_id" in cum_df_outer_left.columns:
             sub_col = cum_df_outer_left.pop("subject_id")
             ses_col = cum_df_outer_left.pop("session_id")
 
+            if collate_prefix_left:
+                orig_cols = cum_df_outer_left.columns.tolist()
+                new_cols = [f"{collate_prefix_left}.{x}" for x in orig_cols]
+                new_dict = dict(zip(orig_cols,new_cols))
+                cum_df_outer_left = cum_df_outer_left.rename(columns=new_dict)
+
             cum_df_outer_left.insert(0,"session_id",ses_col)
             cum_df_outer_left.insert(0,"subject_id",sub_col)
+        elif collate_prefix_left:
+            orig_cols = cum_df_outer_left.columns.tolist()
+            new_cols = [f"{collate_prefix_left}.{x}" for x in orig_cols]
+            new_dict = dict(zip(orig_cols,new_cols))
+            cum_df_outer_left = cum_df_outer_left.rename(columns=new_dict)
 
         cum_df_inner_left.to_csv(roi_csv_inner_left,sep=",",header=True, index=False)
         cum_df_outer_left.to_csv(roi_csv_outer_left,sep=",",header=True, index=False)
 
         metadata = {}
         roi_csv_inner_left_json = os.path.splitext(roi_csv_inner_left)[0] + ".json"
         metadata = updateParams(metadata,"Title","collate_csv_group.py: Inner Join (left hand table)")
@@ -160,34 +184,59 @@
         collate_name_right = getParams(labels_dict,"COLLATE_NAME_RIGHT")
         if not collate_name_right:
             if not pipeline:
                 collate_name_right="csvgroup"
             else:
                 collate_name_right="pipeline"
 
+        collate_prefix_right = getParams(labels_dict,"COLLATE_PREFIX_RIGHT")
+
         roi_csv_inner_right = os.path.join(roi_output_dir,'{}_{}_inner_right.csv'.format("group",collate_name_right))
         roi_csv_outer_right = os.path.join(roi_output_dir,'{}_{}_outer_right.csv'.format("group",collate_name_right))
 
         #create sorted output
         cum_df_inner_right = cum_df_inner_right.reindex(sorted(cum_df_inner_right.columns), axis=1)
         if "session_id" in cum_df_inner_right.columns and "subject_id" in cum_df_inner_right.columns:
             sub_col = cum_df_inner_right.pop("subject_id")
             ses_col = cum_df_inner_right.pop("session_id")
 
+            if collate_prefix_right:
+                orig_cols = cum_df_inner_right.columns.tolist()
+                new_cols = [f"{collate_prefix_right}.{x}" for x in orig_cols]
+                new_dict = dict(zip(orig_cols,new_cols))
+                cum_df_inner_right = cum_df_inner_right.rename(columns=new_dict)
+
             cum_df_inner_right.insert(0,"session_id",ses_col)
             cum_df_inner_right.insert(0,"subject_id",sub_col)
 
+        elif collate_prefix_right:
+            orig_cols = cum_df_inner_right.columns.tolist()
+            new_cols = [f"{collate_prefix_right}.{x}" for x in orig_cols]
+            new_dict = dict(zip(orig_cols,new_cols))
+            cum_df_inner_right = cum_df_inner_right.rename(columns=new_dict)
+
         #create sorted output
         cum_df_outer_right = cum_df_outer_right.reindex(sorted(cum_df_outer_right.columns), axis=1)
         if "session_id" in cum_df_outer_right.columns and "subject_id" in cum_df_outer_right.columns:
             sub_col = cum_df_outer_right.pop("subject_id")
             ses_col = cum_df_outer_right.pop("session_id")
 
+            if collate_prefix_right:
+                orig_cols = cum_df_outer_right.columns.tolist()
+                new_cols = [f"{collate_prefix_right}.{x}" for x in orig_cols]
+                new_dict = dict(zip(orig_cols,new_cols))
+                cum_df_outer_right = cum_df_outer_right.rename(columns=new_dict)
+
             cum_df_outer_right.insert(0,"session_id",ses_col)
             cum_df_outer_right.insert(0,"subject_id",sub_col)
+        elif collate_prefix_right:
+            orig_cols = cum_df_outer_right.columns.tolist()
+            new_cols = [f"{collate_prefix_right}.{x}" for x in orig_cols]
+            new_dict = dict(zip(orig_cols,new_cols))
+            cum_df_outer_right = cum_df_outer_right.rename(columns=new_dict)
 
         cum_df_inner_right.to_csv(roi_csv_inner_right,sep=",",header=True, index=False)
         cum_df_outer_right.to_csv(roi_csv_outer_right,sep=",",header=True, index=False)
 
         metadata = {}
         roi_csv_inner_right_json = os.path.splitext(roi_csv_inner_right)[0] + ".json"
         metadata = updateParams(metadata,"Title","collate_csv_group.py: Inner Join (right hand table)")
@@ -209,17 +258,23 @@
         metadata = updateParams(metadata,"Pipeline",f"{pipeline}")
         metadata = updateParams(metadata,"InputFiles",f"{csv_list_right}")
         export_labels(metadata,roi_csv_outer_right_json)
 
     collate_join_left= getParams(labels_dict,"COLLATECOLS_JOIN_LEFT")
     if not collate_join_left:
         collate_join_left=["subject_id","session_id"]
+    elif collate_prefix_left:
+        collate_join_left = [f"{collate_prefix_left}.{x}" if  f"{collate_prefix_left}." not in x and x != "subject_id" and x != "session_id" else x for x in collate_join_left ]
+
     collate_join_right= getParams(labels_dict,"COLLATECOLS_JOIN_RIGHT")
     if not collate_join_right:
         collate_join_right=["subject_id","session_id"]
+    elif collate_prefix_right:
+        collate_join_right = [f"{collate_prefix_right}.{x}" if  f"{collate_prefix_right}." not in x and x != "subject_id" and x != "session_id" else x for x in collate_join_right ]
+
 
     if not cum_df_inner_right.empty and not cum_df_inner_left.empty:
         cum_df_inner = pd.merge(cum_df_inner_left, cum_df_inner_right,  how='left', left_on=collate_join_left, right_on =collate_join_right)
         roi_csv_inner = os.path.join(roi_output_dir,'{}_{}-{}_inner.csv'.format("final-group",collate_name_left,collate_name_right))
 
         #create sorted output
         cum_df_inner = cum_df_inner.reindex(sorted(cum_df_inner.columns), axis=1)
```

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/collate_csv_single.py` & `panpipelines-1.0.2/src/panpipelines/nodes/collate_csv_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/dummy.py` & `panpipelines-1.0.2/src/panpipelines/nodes/dummy.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/fmriprep.py` & `panpipelines-1.0.2/src/panpipelines/nodes/fmriprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/freesurfer.py` & `panpipelines-1.0.2/src/panpipelines/nodes/freesurfer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/fslanat.py` & `panpipelines-1.0.2/src/panpipelines/nodes/fslanat.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/glm_randomize_group.py` & `panpipelines-1.0.2/src/panpipelines/nodes/glm_randomize_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/lst.py` & `panpipelines-1.0.2/src/panpipelines/nodes/lst.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/mriqc.py` & `panpipelines-1.0.2/src/panpipelines/nodes/mriqc.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/noddi.py` & `panpipelines-1.0.2/src/panpipelines/nodes/noddi.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/parse_textdata.py` & `panpipelines-1.0.2/src/panpipelines/nodes/parse_textdata.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/preproc.py` & `panpipelines-1.0.2/src/panpipelines/nodes/preproc.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/qsiprep.py` & `panpipelines-1.0.2/src/panpipelines/nodes/qsiprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/roi_extract.py` & `panpipelines-1.0.2/src/panpipelines/nodes/roi_extract.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/roi_mean_group.py` & `panpipelines-1.0.2/src/panpipelines/nodes/roi_mean_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/roi_mean_single.py` & `panpipelines-1.0.2/src/panpipelines/nodes/roi_mean_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/nodes/tensor.py` & `panpipelines-1.0.2/src/panpipelines/nodes/tensor.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/aslprep_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/aslprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/basil_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/basil_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/collatecsv_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/collatecsv_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/dummy_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/dummy_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/fmriprep_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/fmriprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/freesurfer_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/freesurfer_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/lst_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/lst_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/mriqc_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/mriqc_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/noddi_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/noddi_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/preproc_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/preproc_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/qsiprep_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/qsiprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/roiextract_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/roiextract_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/tensor_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/tensor_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/textmeasures_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/textmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/pipelines/volmeasures_panpipeline.py` & `panpipelines-1.0.2/src/panpipelines/pipelines/volmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/scripts/aslprep_panscript.py` & `panpipelines-1.0.2/src/panpipelines/scripts/aslprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/scripts/fmriprep_panscript.py` & `panpipelines-1.0.2/src/panpipelines/scripts/fmriprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/scripts/mne_make_surfaces.py` & `panpipelines-1.0.2/src/panpipelines/scripts/mne_make_surfaces.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/scripts/pancontainer_panscript.py` & `panpipelines-1.0.2/src/panpipelines/scripts/pancontainer_panscript.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from panpipelines.utils.util_functions import *
 from panpipelines.scripts.panscript import *
 
 
 class pancontainer_panscript(panscript):
 
-    def __init__(self,labels_dict,name='pancontainer_panscript',params="",command="",container_img="PAN_CONTAINER",execution={}):
-        super().__init__(labels_dict,name=name,params=params,command=command)
+    def __init__(self,labels_dict,name='pancontainer_panscript',params="",command="",interactive=False,container_img="PAN_CONTAINER",execution={}):
+        super().__init__(labels_dict,name=name,params=params,command=command,interactive=interactive)
 
         self.params = params
 
         if not container_img:
             container_img = "PAN_CONTAINER"
 
         command_base, container = getContainer(labels_dict,nodename="pancontainer_panscript",SPECIFIC=container_img,LOGGER=IFLOGGER)
```

### Comparing `panpipelines-1.0.1/src/panpipelines/scripts/panscript.py` & `panpipelines-1.0.2/src/panpipelines/scripts/panscript.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import os
 from nipype import logging as nlogging
 
 IFLOGGER=nlogging.getLogger('nipype.interface')
 
 class panscript:
 
-    def __init__(self,labels_dict,name='template_panscript',params="",command="",execution={}):
+    def __init__(self,labels_dict,name='template_panscript',params="",command="",interactive=False, execution={}):
 
         # Create Node
         self.labels_dict = labels_dict
         self.name = name
         self.params = params
         self.command = command
+        self.interactive = interactive
 
 
     def pre_run(self):
         pass
 
     def run(self):
 
@@ -27,15 +28,15 @@
         command=self.command + " " + self.params
 
         pkgdir = os.path.abspath(os.path.dirname(__file__))
         IFLOGGER.info(f"Changing to panscript directory {pkgdir} to execute.")
         os.chdir(pkgdir)
         
         evaluated_command=substitute_labels(command, self.labels_dict)
-        runCommand(evaluated_command,IFLOGGER)
+        runCommand(evaluated_command,IFLOGGER,interactive=self.interactive)
 
         self.post_run()
         return self.get_results()
 
     def post_run(self):
         pass
```

### Comparing `panpipelines-1.0.1/src/panpipelines/scripts/sdcflows_fieldmap.py` & `panpipelines-1.0.2/src/panpipelines/scripts/sdcflows_fieldmap.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/utils/transformer.py` & `panpipelines-1.0.2/src/panpipelines/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/utils/util_functions.py` & `panpipelines-1.0.2/src/panpipelines/utils/util_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,37 @@
 
 def drop_ses(value):
     return re.sub(r"^ses-", "", str(value))
 
 def isTrue(arg):
     return arg is not None and (arg == 'Y' or arg == 'y' or arg == '1' or arg == 'True' or arg == 'true' or arg == True)
 
+def special_substitution(expression,pardict, key,unbracedKey):
+    if expression is not None and key is not None and pardict is not None:
+        if key=="<XNAT_USER>":
+            credentials = os.path.abspath(getParams(pardict,"CREDENTIALS"))
+            if credentials is not None and os.path.exists(credentials):
+                with open(credentials, 'r') as infile:
+                    cred_dict = json.load(infile)
+                    if "user" in cred_dict.keys():
+                        cred_user = getParams(cred_dict,"user")
+                        expression = expression.replace(key,cred_user) 
+        elif key=="<XNAT_PASSWORD>":
+            credentials = os.path.abspath(getParams(pardict,"CREDENTIALS"))
+            if credentials is not None and os.path.exists(credentials):
+                with open(credentials, 'r') as infile:
+                    cred_dict = json.load(infile)
+                    if "password" in cred_dict.keys():
+                        cred_password = getParams(cred_dict,"password")
+                        expression = expression.replace(key,cred_password)
+        elif unbracedKey in pardict and isinstance(pardict[unbracedKey],list):
+            list_string = " ".join(pardict[unbracedKey])
+            expression = expression.replace(key,list_string)
+    return expression
+
 def getParams(pardict, key, update=True):
     if key is not None and pardict is not None:
         if key in pardict:
             if update:
                 updateParams(pardict,key,pardict[key])
                 return pardict[key] 
             else:
@@ -132,14 +155,25 @@
 
     return pardict
 
 def export_labels(panpipe_labels,export_file):
     with open(export_file,"w") as outfile:
         json.dump(panpipe_labels,outfile,indent=2)
 
+def special_substitute_labels(expression,panpipe_labels,exceptions=[]):
+    if isinstance(expression,str):
+        braced_vars = re.findall(r'\<.*?\>',expression)
+        for braced_var in braced_vars:
+            unbraced_var = braced_var.replace('<','').replace('>','')
+            lookup_var = getParams(panpipe_labels,unbraced_var)
+            if isinstance(lookup_var,str) and lookup_var is not None and unbraced_var not in exceptions:
+                expression = expression.replace(braced_var,lookup_var) 
+            else:
+                expression = special_substitution(expression, panpipe_labels,braced_var,unbraced_var)           
+    return expression
 
 def substitute_labels(expression,panpipe_labels,exceptions=[]):
     if isinstance(expression,str):
         braced_vars = re.findall(r'\<.*?\>',expression)
         for braced_var in braced_vars:
             unbraced_var = braced_var.replace('<','').replace('>','')
             lookup_var = getParams(panpipe_labels,unbraced_var)
@@ -2067,14 +2101,16 @@
 
 
 def getContainer(labels_dict,nodename="",SPECIFIC=None,CONTAINERALT="PAN_CONTAINER", LOGGER=UTLOGGER):
     if SPECIFIC:
         container_run_options = getParams(labels_dict,f"{SPECIFIC}_RUN_OPTIONS")
         container_prerun = getParams(labels_dict,f"{SPECIFIC}_PRERUN")
         container = getParams(labels_dict,f"{SPECIFIC}")
+        if SPECIFIC == "DUMMY_CONTAINER":
+            return "",""
     else:
         container_run_options = None
         container_prerun = None
         container = None
 
     if container and not container_run_options:
         container_run_options = getParams(labels_dict,'CONTAINER_RUN_OPTIONS')
```

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/aslprep_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/aslprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/basil_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/basil_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/collatecsv_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/collatecsv_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/collatecsvgroup_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/collatecsvgroup_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/dummy_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/fmriprep_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/fmriprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/freesurfer_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/lst_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/lst_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/mriqc_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/mriqc_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/noddi_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/noddi_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/preproc_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/preproc_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/qsiprep_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/qsiprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/roiextract_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/roiextract_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/tensor_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/tensor_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/textmeasures_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/textmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/src/panpipelines/workflows/volmeasures_workflow.py` & `panpipelines-1.0.2/src/panpipelines/workflows/volmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/.gitignore` & `panpipelines-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/LICENSE` & `panpipelines-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/README.md` & `panpipelines-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/pyproject.toml` & `panpipelines-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpipelines-1.0.1/PKG-INFO` & `panpipelines-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpipelines
-Version: 1.0.1
+Version: 1.0.2
 Summary: MRI Processing Pipelines for PAN Healthy Minds for Life Study
 Project-URL: Homepage, https://github.com/MRIresearch/PANpipelines
 Project-URL: Bug Tracker, https://github.com/MRIresearch/PANpipelines/issues
 Author-email: Chidi Ugonna <chidiugonna@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 MRIresearch
```

