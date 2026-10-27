laselva_v1 audio (data-prep repo, kaanturan3/data-prep)
========================================================

This archive is the audio_root for datasets/laselva_v1. Unzip it anywhere; the
folder that contains "macaulay/" and "data-prep/" is the audio root.

  macaulay/flac/      3,179 Macaulay Library recordings from La Selva, FLAC 32 kHz mono 16-bit
  data-prep/xc_flac/  77 Xeno-canto set 2146 recordings, FLAC 32 kHz mono 16-bit

Every "path" in datasets/laselva_v1/manifest.csv is relative to this folder:

  from scripts.load_dataset import load_dataset
  df = load_dataset("datasets/laselva_v1", audio_root="/path/to/unzipped/folder")

Converted from the originals with scripts/convert_to_flac.py. Clip metadata
(species, checklist, recordist, date, rating, duration) is in manifests/ml_la_selva.csv
and manifests/xc_set_2146.csv in the repo; see HANDOVER.md.

Terms
-----
Macaulay Library audio (Cornell Lab of Ornithology): research use within the
ECE 534 project team. Credit "Cornell Lab of Ornithology | Macaulay Library" and
cite clips as "Species (ML#####)". Do not repost or redistribute outside the team.
Xeno-canto audio: CC BY-NC-SA 4.0, recordist Bobby Wilcox; cite catalog numbers (XC#####).
