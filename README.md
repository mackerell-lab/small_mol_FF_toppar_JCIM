<h1 align="center">Small Molecule ForceField Toppar Files </h1>


This is a collection of topology and parameter files generated for `264` ligands by parameter assignment programs. The investigated parameter assignment programs and generalized force fields are tabulated below:


| Parameter Assignment Program | Charge Model | Force Field  | Parameter Set |
| ---------------------------- | ------------ | ------------ | ------------- |
| CGenFF v 2.5.1               | N/A          | CGenFF v4.6  | CGenFF        |
| CGenFF legacy v 1.0          | N/A          | CGenFFv3.0.1 | CGenFF Legacy |
| MATCH v 0.01                 | N/A          | CGenFFv3.0.1 | MATCH/CGenFF  |
| Antechamber, AmberTools21    | RESP         | GAFF2.11     | GAFF2/RESP    |
| Antechamber, AmberTools21    | AM1-BCC      | GAFF2.11     | GAFF2/AM1-BCC |
| Antechamber, AmberTools21    | AM1-BCC      | GAFF1.81     | GAFF/AM1-BCC  |

In addition to the parameter sets above, we investigated the modified `CGenFFv3.0.1`, modified `GAFF2.11`, and `OpenFF 1.2.0 Parsley` topologies and parameters provided by [Gapsys et al, J. Chem. Inf. Model. 2022](doi.org/10.1021/acs.jcim.1c01445).

Data pertaining to Gasys et al are provided in the respective [GitHub repository](https://github.com/deGrootLab/rel_ddG_MerckDataSet_JCIM).

## Contents
```
├── cgenff
│   ├── ligand_id
│   │   ├── mol.str (CGenFF stream file output)
├── cgenff_legacy
│   ├── ligand_name
│   │   ├── mol.str (CGenFF Legacy stream file output)
├── match_cgenff
│   ├── ligand_id
│   │   ├── mol.rtf (MATCH topology file output)
│   │   ├── mol.prm (MATCH parameter file output)
│   │   ├── mol.log (MATCH log output)
├── gaff_am1_bcc
│   ├── ligand_id
│   │   ├── mol_am1bcc_gaff.ac (Antechamber topology file output)
│   │   ├── mol_gaff.frcmod (Antechamber parameter file output)
├── gaff2_am1_bcc
│   ├── ligand_id
│   │   ├── mol_am1bcc_gaff2.ac (Antechamber topology file output)
│   │   ├── mol_gaff2.frcmod (Antechamber parameter file output)
├── gaff2_am1_bcc
│   ├── ligand_id
│   │   ├── resp_charges.txt (RESP charges)
└── └── └── mol_gaff2.frcmod (Antechamber parameter file output)
```
Ligand IDs are based on the naming provided in [Gapsys et al, J. Chem. Inf. Model. 2022](doi.org/10.1021/acs.jcim.1c01445), which include the protein system the ligands are associated with followed by their ligand name.

RESP charges were calculated through `Psi4` and workflows developed in [Kumar et al, J. Chem. Theory Comput. 2022](doi.org/10.1021/acs.jctc.1c01166).

## Citation

Asuka A. Orr, Suliman Sharif, Junmei Wang, Alexander D. MacKerell Jr. Preserving the Integrity of Empirical Force Fields. _Under Review_.
