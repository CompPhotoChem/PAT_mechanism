### `esa` — Excited-State Absorption

Contains excited-state absorption properties for different electronic transitions.

- **S₁ → Sₙ transitions** of **1a** via ADC(2)
  - *Computational details* (Turbomole 7.7): ADC(2)/def2-TZVP, COSMO(THF)

- **T₁ → Tₙ transitions** of **1b** via TD-DFT
  - *Computational details* (Gaussian 16W):
    ```
    td=(triplets, nstates=10) b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene)
    ```

**File structure**:
- **1st column**: vertical transition energies (in eV)
- **2nd column**: oscillator strengths
