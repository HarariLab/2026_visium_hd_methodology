## SpaceRanger (v3.1.3) Visium HD alignments scripts
Folder contains bsub scripts to run SpaceRanger on OSC HPC for three sample batches.
Bsub script uses associated metadata file to define SpaceRanger parameters

### FFPE Pilot
Samples:
- ffpeAD2_S3
- ffpeAD3_S1

```
sbatch spaceranger_hd_ffpe_pilot.bsub
```

### FF Pilot
Samples:
- AD2_S1
- AD2_S2

Contains two parts: first sequencing round on Nov 2025 and additional sequencing round for the same libraries on Dec 2025
```
# Reads from first sequencing round
sbatch spaceranger_hd_ff_pilot_nov25.bsub
```

```
# Combined (topped up) reads from both sequencing rounds
sbatch spaceranger_hd_ff_pilot_dec25_topped.bsub
```

### FF Batch1
Samples:
- AD3_S1
- AD4_S1
- AD5_S1

```
sbatch spaceranger_hd_ff_batch1_mar26.bsub
```