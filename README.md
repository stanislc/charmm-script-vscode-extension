# CHARMM Script VS Code Extension

Comprehensive syntax highlighting for CHARMM (Chemistry at HARvard Macromolecular Mechanics) input scripts.

## Features

This extension provides extensive syntax highlighting for CHARMM `.inp` and `.str` files, covering:

### Command Categories

- **Main Commands**: `DYNA`, `MINI`, `ENER`, `VIBR`, `CORR`, `TRAJ`, etc.
- **Dynamics**: `NOSE`, `SHAKE`, `MTS`, `TAMD`, `TMD`, `REPLICA`, `DOMDEC`, dynamics options
- **Energy**: `BLOC`, `MMFP`, `CONS`, `PERT`, energy terms (bond, angle, dihedral, vdw, elec, etc.)
- **Structure**: `READ`, `GENE`, `PATC`, `DELE`, `RENA`, `JOIN`, `DRUD`, `LONE`
- **Coordinates**: `COOR` subcommands (init, copy, rotate, translate, rms, stat, etc.)
- **I/O**: `OPEN`, `CLOSE`, `READ`, `WRITE`, `PRINT`, `TRAJ`, file formats
- **Analysis**: `ANAL`, `CORREL`, `NMR`, `NOE`, `RDC`, `ESTATS`
- **Solvation**: `GBMV`, `GBSW`, `PBEQ`, `EEF1`, `SASA`, `IMAGE`, `CRYSTAL`
- **QM/MM**: `QUANTUM`, `GAMESS`, `GAUSSIAN`, `QCHEM`, `SCCDFTB`, `DRUDE`, `CHEQ`
- **Miscellaneous**: `BLADE`, `OPENMM`, `DOMDEC`, `MC`, `CSA`, `EMAP`, etc.

### Syntax Elements

- **Control Flow**: `IF/THEN/ELSE/ENDIF`, `GOTO`, `LABEL`, `STREAM`, `RETURN`, `STOP`
- **Variables**: `@variable` references and `?query` variables
- **Operators**: `.EQ.`, `.NE.`, `.LT.`, `.GT.`, `.LE.`, `.GE.`, `.AND.`, `.OR.`, `.NOT.`
- **Selection Keywords**: `SELE`, `END`, `SEGID`, `RESID`, `RESN`, `ATOM`, `TYPE`, `.AROUND.`, `.BONDED.`
- **Storage**: `SET`, `DEFINE`, `CALC`, `SCALAR`
- **Constants**: Integer, float, scientific notation, boolean values
- **Comments**: `!` line comments and `*` title lines

## Supported File Extensions

- `.inp` - CHARMM input files
- `.str` - CHARMM stream files
- `.rtf` - Residue Topology Files
- `.prm` - Parameter files
- `.crd` - Coordinate files
- `.psf` - Protein Structure Files

## Installation

### From VSIX (Local)
1. Download or build the `.vsix` file
2. In VS Code: Extensions > ... > Install from VSIX

### From Source
1. Clone this repository
2. Copy to your VS Code extensions folder:
   - Windows: `%USERPROFILE%\.vscode\extensions\`
   - macOS/Linux: `~/.vscode/extensions/`
3. Restart VS Code

## Building

```bash
npm install -g @vscode/vsce
vsce package
```

## Release Notes

### 1.0.0

Major enhancement release:
- Added 200+ CHARMM commands organized into categories
- Variable highlighting (`@var` and `?var`)
- Selection keyword support
- Improved number matching (floats, scientific notation)
- Added `.str` file extension support
- Case-insensitive matching for all keywords

### 0.0.1

Initial alpha release

## Credits

- Original extension by [Truman-Xu](https://github.com/Truman-Xu)
- Enhanced with comprehensive command coverage based on CHARMM source code analysis

## License

MIT License
