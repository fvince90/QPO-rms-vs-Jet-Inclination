# Type-C QPO Fractional RMS Catalog for Black Hole X-ray Binary Transients

A living catalog of type-C quasi-periodic oscillation (QPO) fractional rms amplitudes measured in the 2–25 keV band during the rising hard state of black hole X-ray binary transients. The sample is restricted to systems with jet inclination angles constrained from resolved ballistic jet proper motions. 

**Latest update:** 27 May 2026

## Catalog description

The file `qpo_rms_catalog.csv` contains the following columns:

| Column | Description |
|---|---|
| `Satellite` | X-ray observatory used for the timing measurement (RXTE or HXMT) |
| `Source` | Source name |
| `i_jet_deg` | Jet inclination angle to the line of sight (degrees) |
| `i_jet_err` | Uncertainty on jet inclination; upper limits indicated with `<` prefix, asymmetric errors as `+X/-Y` |
| `BH_Mass_Msun` | Black hole mass estimate (solar masses); ranges given as `X-Y`, lower limits as `>X` |
| `rms_lt1Hz_pct` | Mean fractional rms (%) for QPOs with frequency < 1 Hz |
| `rms_lt1Hz_err` | 1σ uncertainty on the above |
| `N_lt1Hz` | Number of QPO detections in this frequency bin |
| `rms_1to4Hz_pct` | Mean fractional rms (%) for QPOs with frequency 1–4 Hz |
| `rms_1to4Hz_err` | 1σ uncertainty |
| `N_1to4Hz` | Number of QPO detections |
| `rms_4to8Hz_pct` | Mean fractional rms (%) for QPOs with frequency 4–8 Hz |
| `rms_4to8Hz_err` | 1σ uncertainty |
| `N_4to8Hz` | Number of QPO detections |
| `rms_8to10Hz_pct` | Mean fractional rms (%) for QPOs with frequency 8–10 Hz |
| `rms_8to10Hz_err` | 1σ uncertainty |
| `N_8to10Hz` | Number of QPO detections |
| `i_jet_ref` | Reference for the jet inclination measurement (ADS bibcode in parentheses) |
| `mass_ref` | Reference for the black hole mass estimate (ADS bibcode in parentheses) |

Empty cells indicate that no measurement is available for that source and frequency bin.

## Sample selection

Sources are included if and only if:

1. They are confirmed or strong black hole X-ray binary transient candidates.
2. Their jet inclination angle has been constrained through modelling of the proper motion of resolved discrete (ballistic) jet ejecta.
3. Type-C QPOs have been detected during the rising hard state.

## Data provenance

- **RXTE sources**: QPO parameters extracted from RXTE/PCA archival observations.
- **Insight-HXMT sources**: QPO parameters extracted from Insight-HXMT archival observations.
- All rms values are fractional rms amplitudes computed in the 2–25 keV energy band.
- QPOs are averaged within four frequency bins: <1 Hz, 1–4 Hz, 4–8 Hz, and 8–10 Hz. The number in the `N` column indicates how many individual QPO detections were averaged.

## How to cite

If you use this catalog in your research, please cite:

> Vincentelli, Bollemeijer, Veledina et al. (2026), *The strength of Type-C quasi-periodic oscillations in black hole X-ray binaries correlates with the jet inclination* (MNRAS, accepted, arxiv link in prep.)

and the individual references listed in the `i_jet_ref` and `mass_ref` columns for the specific sources you use.

A BibTeX entry is provided in `CITATION.cff` and `CITATION.bib`.
