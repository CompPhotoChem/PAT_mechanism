### `scan` — Potential Energy Surface Scans

- `PES_1b_relScan-T1_b3lyp.dat`: Relaxed scan of the **SC=CS** dihedral angle on the **T₁** surface for **1b**.
Simulated over a range of 180° to 0° in 5° steps.
  - *Computational details* (Gaussian 16W):
    ```
    b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene) # for T1 and S0
    td=(singlets, nstates=10) b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene) # for S1 and S2
    td=(triplets, nstates=10) b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene) # for T2
    ```

- `PES_1b-E_1b-Z_S0min_b3lyp.dat`: Relative energies of S₀, S₁, S₂, T₁, and T₂ at the equilibrium geometries of **1b-E** and **1b-Z**.
  - *Computational details* (Gaussian 16W):
    ```
    b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene) # for T1 and S0
    td=(singlets, nstates=10) b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene) # for S1 and S2
    td=(triplets, nstates=10) b3lyp/6-311g(d,p) scrf=(iefpcm,solvent=benzene) # for T2
    ```

**File structure**:
- **1st column**: SC=CS dihedral angle (in °)
- **2nd column**: relative energy of **S₀** (in eV, relative to S₀ minimum of 1b-E)
- **3rd column**: relative energy of **S₁** (in eV)
- **4th column**: relative energy of **T₁** (in eV)
- **5th column**: relative energy of **T₂** (in eV)
- **6th column**: relative energy of **S₂** (in eV)
- **7th column**: spin–orbit coupling between **S₀** and **T₁** (in cm⁻¹)
