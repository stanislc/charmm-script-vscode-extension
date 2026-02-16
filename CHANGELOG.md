# Change Log

All notable changes to the "charmm-script" extension will be documented in this file.

## [1.0.0] - 2026-01-22

### Added
- 200+ CHARMM commands organized into 15 categories
- Variable highlighting for `@variable` and `?query` syntax
- Selection keywords (SELE, SEGID, RESID, etc.) and operators (.AND., .OR., .NOT., etc.)
- Dynamics commands: NOSE, SHAKE, MTS, TAMD, REPLICA, DOMDEC, etc.
- Energy commands: BLOC, CONS, PERT, energy terms (bond, angle, vdw, elec, etc.)
- Solvation commands: GBMV, GBSW, PBEQ, EEF1, SASA, IMAGE, CRYSTAL, etc.
- QM/MM commands: QUANTUM, GAMESS, GAUSSIAN, QCHEM, SCCDFTB, DRUDE, etc.
- Analysis commands: CORREL, NMR, NOE, RDC, ESTATS, etc.
- Subcommands for COOR, IC, SCALAR, and other modules

### Changed
- Improved number matching to support floats and scientific notation
- Case-insensitive matching for all keywords
- Better comment detection (both `!` and `*` styles)

### Extended
- File extension support: `.inp`, `.str`, `.rtf`, `.prm`, `.crd`, `.psf`

## [0.0.1] - Initial Release

- Alpha release with basic syntax highlighting
