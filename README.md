# protein-mutation-data

This dataset contains protein information, structural information, experimental conditions, experimental thermodynamic data, and literature references on protein wildtypes and mutants. It is gathered from the following three databases.

## Sources:

### **ProTherm Database**:
The ProTherm Database is the larges Protein thermodynamic database with approximately 31,000 entries. It contains protein wildtype and mutant stability data, structural data, and literature references. The data has been compiled from various other databases (e.g. BRENDA, PubMed), manually curated from literature or directly submitted to the database.

Link to Database: https://web.iitm.ac.in/bioinfo2/prothermdb/index.html

Link to Literature: https://academic.oup.com/nar/article/49/D1/D420/5983626

### **ThermoMut Database**:
The ThermoMut Database contains approximately 13,000 entries. It contains protein (wildtype and mutant) information, experimental conditions, thermodynamic data, structural environment data, substitution matrices scores, pharmacophore changes data, and literature information. Only protein information, experimental conditions, thermodynamic data, and literature information were included in the Protein Mutation database. The data in the ThermoMut Database derives from the ProTherm Database, manually curated data, and directly submitted experimental data.

Link to Database: http://biosig.unimelb.edu.au/thermomutdb/

Link to Literature: https://academic.oup.com/nar/article/49/D1/D475/5937085?login=true

### **Fireprot Database**:

The FireProt Database contains approximately 17,000 entries of single-point protein mutant stability data, literature information, and sequence and structure annotations. The data was gathered from the ProTherm database, ProtaBank, directly submitted experimental data, and manually curated data. Sequence and structure annotations on data were made using VariBench and Hotspot Wizard.

Link to Database: https://loschmidt.chemi.muni.cz/fireprotdb/

Link to Literature: https://academic.oup.com/nar/article/49/D1/D319/5964070


## Protein Stability Dataset Column Names:
 **DATABASE**: Database from which data was derived from. (e.g. "Protherm")

 **PROTEIN**: Protein name for which row pertains to. (e.g. "Lysozyme")

 **UNIPROT_ID**: UniProtKB/Swiss-Prot database ID. (e.g. P00720)

 **MUTATION**: Protein mutation code. (e.g. D26N)

 **SOURCE**: Protein organism. (e.g. Homo sapien)

 **PBD_WILD**: Protein Data Bank ID for protein. (e.g 1WQ5)

 **PBD_CHAIN_MUTATION**: Details Protein Data Bank ID, mutated chain, and mutation in PBD formatting.  (e.g 1wq5_A:M101V)

**pH**: Experimental pH. (e.g 7.0)

**T_(C)**: Experimental temperature in degree Celsius. (e.g 25)

**Tm_(C)**: Melting temperature -
temperature at which the concentration of the protein
in folded state equals the concentration of the unfolded protein.(e.g 53.1)

**dTm_(C)**: The change in melting temperature in Celsius. (e.g -6.4)

**dH_(kcal/mol)**: The change in enthalpy of denaturation in kcal/mol. (e.g. 119.5)

**dG_(kcal/mol)**: The change in Gibbs free energy in kcal/mol. (e.g. 1.44)

**ddG_(kcal/mol)**: (dG(mutant) - dG(wild)) The variation of Gibbs Free Energy in kcal/mol. A positive value corresponds to stabilizing mutations, and a negative value corresponds to destabilized mutations. (e.g. -3.2)

**ddG_H2O_(kcal/mol)**: (dG_H2O(mutant) - dG_H2O(wild)). Change in Free Energy of unfolding in water in kcal/mol. (e.g. -2.31)

**STATE**: Number of transition states. (e.g. 3)

**REVERSIBILITY**: Reversibility of reaction. (e.g. yes)

**PUBMED_ID**: Publication ID in PubMed Database. (e.g. 9551101)

**REFERENCE**: Publication reference to article/journal. (e.g J MOL BIOL 3, 625-46 (1998))

**KINGDOM**: Kingdom from which source originated. (e.g. Eukaryota)

**PBD_mutant**: PDB code for mutant (e.g. 1L54)

**MUTATED_CHAIN**: Chain in which mutation occurred. (e.g. A)

**MEASURE**: Experimental technique for studying folding. (e.g. Fluorescence)

 **METHOD**: Technique to denature protein. (e.g.Thermal)

 **POSITION**: Location of protein mutation. (e.g. 8)

 **WILD_TYPE_RES**: Single letter wild-type residue before mutation. (e.g. L)

 **MUTATED_RES**: Single letter mutated residue after mutation. (e.g. S)

 **IS_CURATED**: Boolean value of whether reference is curated. (e.g. TRUE)

 **CONSERVATION**: Evolutionary conservation score - Calculated per base and indicates how many species in a given multiple alignment match at each locus. (e.g. 3)

**NOTES**: miscellaneous notes about experiment (e.g. cysteine-free variant)

**DATASETS**: Datasets where data derived from. (e.g khan1784)

## Reaction Datasets Column Names:

## Sources:

### **SABIO-RK Database**:


Link to Database:

Link to Literature:

## CSV Files/Source Code:
