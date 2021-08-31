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

## Sources:

### **MuteinDB**:
The Mutein Database contains approximately 500 entries of experimental data about muteins and their biochemical properties (including kinetic data on catalyzed reactions). It is sourced from publicly available sources and directly submitted experimental data.

Link to Database: https://muteindb.genome.tugraz.at/muteindb-web-2.0/faces/init/index.seam

Link to Literature: https://academic.oup.com/database/article/doi/10.1093/database/bas028/436165

### **SABIO-RK Database**:
The SABIO-RK Database contains approximately 70,000 data entries on biochemical reactions and their reaction kinetics, and is sourced from manually curated scientific literature.

Link to Database: http://sabio.h-its.org/

Link to Literature: https://academic.oup.com/nar/article/46/D1/D656/4577570

## SABIO_RK Reaction Dataset Column Names:


**EntryID**: Reaction ID in SABIO-RK database. (e.g. 53)

**Reaction**: Biochemical reaction occurring in experiment. (e.g. e- + H+ = Hydrogen)

**Organism**: Organism from which enzyme is derived from. (e.g. gallus gallus)

**ECNumber**: EC Number classification of enzyme used in reaction. (e.g. 3.2.1.17)

**paramter.type**: Type of parameter measurement in reaction. (e.g. concentration)

**parameter.associatedSpecies**: Species that parameter.type is measuring (e.g. Enzyme)

**parameter.startValue**: Initial value of parameter before experiment. (e.g. 0.0)

**parameter.endValue**: Final value of parameter after experiment (e.g. 100.0)

**parameter.standardDeviation**: Standard deviation of parameter measurements (e.g. 0.1)

**parameter.unit**: Unit paramter.type is measured in (e.g. mM)

**UniProtKB_AC**: UniProtKB_AC of enzyme. (e.g. P00698)

**Enzyme Variant**: Enzyme wild-type or mutant name (e.g. wild-type)

**Enzymename**: Name of enzyme. (e.g. dihydrofolate reductase)

**Publication**: Publication information of experiment (e.g van Haaster DJ, Hagedoorn PL, . . .)

**PubMedID**: Publication ID in PubMed Database. (e.g. 15667251.0)

**Substrate**: Substrate in reaction (e.g. Hydrogen)

**Product**: Product in reaction (e.g. e-, H+)

**Temperature**:  Experimental temperature in degree Celsius. (e.g 25.0)

**pH**: Experimental pH. (e.g 7.0)

**Rate Equation**: Equation used to calculate rate value in experiment (e.g. kcat*S/(Km+S))


## Files/Source Code Descriptions:

**DBData**:
 - _SABIO-RK_: Folder with data downloaded from the SABIO-RK database
 - _ProThermDB_30_JUN_21.tsv_: Raw ProthermDB data.
 - _all_data_clean.csv_: Cleaned and compiled data from ProthermDB, ThermoMutDB, and FireProtDb; contains 37, 764 rows.
 - _all_data_raw.csv_: NOT cleaned and compiled data from ProthermDB, ThermoMutDB, and FireProtDb; contains 60, 620 rows.
 - _fireprotdb_results.csv_: Raw FireProtDB data.
 - _muteindb.csv_: Raw MuteinDB data.
 - _muteindb_clean.csv_: Cleaned MuteinDB data with 485 rows.
 - _sabio-rk_raw_: Compiled 2000-2021 data from SABIO-RK database with 179, 773 rows.
 - _thermomutdb.csv_: Raw ThermoMutdb data.


 **Adding Enzyme Columm.ipynb**: Jupyter notebook with code to add enzyme column to all_data_clean.csv. NOTE: uniprot-v3 is not included because file is too large

 **Cleaning and Formatting Protein Mutation Data.ipynb**: Jupyter notebook with code to clean and compile Protein Stability Dataset and MuteinDB data.

 **ML Script Generation.ipynb**: Jupyter notebook with script to format a given protein's mutations and parameter into txt file.

 **SABIO-RK Notebook**: Jupyter notebook with query to SABIO-RK data and compilation into sabio-rk_raw
