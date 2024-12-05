# NuGrid Data Releases

## Overview of available models

* **Set1** ([Pignatari *et al.* 2016](http://adsabs.harvard.edu/abs/2016ApJS..225...24P)). AGB and massive stars for metallicities Z = 0.02,  0.01.
* **Set1ext** ([Ritter *et al.* 2018](http://adsabs.harvard.edu/abs/2018MNRAS.480..538R)). Extension of Set1. New Z = 0.006, 0.001, 0.0001. New masses at all metallicities. All models computed with MESA.
* **Set1upd** ([Battino *et al.* 2019](https://academic.oup.com/mnras/article/489/1/1082/5552141), [Battino et al. 2021](https://www.mdpi.com/2218-1997/7/2/25)). Update for low-mass AGB models (M = 2 and 3 Msun) for existing metallicities (Z = 0.02, 0.01, 0.001) and new metallicities (Z = 0.03, 0.002).
* **super-AGB** ([Jones *et al.*
  2016](https://doi.org/10.1093/mnras/stv2488)), super-AGB evolution with H
  ingestion into the He-burning convection zones.
* **Radioactive isotopes ccSN** ([Lawson *et al*
  2022](https://doi.org/10.1093/mnras/stab3684)), Analysis of yields from 62
  core-collapse supernovae models
* **iRAWD** ([Stephens *et al* 2021](https://doi.org/10.1093/mnras/stab500)),
  *i*-process in rapidly accreting white dwarfs (RAWD)

* **Type Ia SN** ([Keegans *et al*]()), common envelope

## DATA ACCESS

NuGrid data are publically available (see below), and can be analyzed online via the Cyberhubs instance [WENDI](http://wendi.nugridstars.org).

## Recommended single stellar nucleosynthesis dataset
This is the recommended NuGrid stellar models and ejected yields dataset. We recommend using this dataset for various purposes, such as inputs for GCE simulations, comparisons with observations and laboratory data, and more.


| **Z = 0.03**           |            | |  | 
|----------------|------------|------------|------------|
| M = 2 Msun       | [Yields](https://nugrid.github.io/files/yields_tables/m2m3_z1m2_z2m2_z3m2_Battino2019.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z3m2_z2m2_z1m2_final_surf_isoabu_Battino2019.txt)  | Battino et al. 2019
| M = 3 Msun       | [Yields](files/yields_tables/m2m3_z1m2_z2m2_z3m2_Battino2019.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z3m2_z2m2_z1m2_final_surf_isoabu_Battino2019.txt)  | Battino et al. 2019
| | | | |
| **Z = 0.02**           |            | |  | 
| M = 1 Msun       | [Yields](files/yields_tables/m1_z2m2_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1z2m2_fin_surfabu.dat)  | Ritter et al. 2018
| M = 1.65 Msun       | [Yields](files/yields_tables/m1p65_z2m2_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1p65z2m2_fin_surfabu.dat)  | Ritter et al. 2018
| M = 2 Msun       | [Yields](files/yields_tables/m2m3_z1m2_z2m2_z3m2_Battino2019.txt) | [Final surface abundances](files/final_surf_abu/m2m3_z3m2_z2m2_z1m2_final_surf_isoabu_Battino2019.txt)  | Battino et al. 2019
| M = 3 Msun       | [Yields](files/yields_tables/m2m3_z1m2_z2m2_z3m2_Battino2019.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z3m2_z2m2_z1m2_final_surf_isoabu_Battino2019.txt)   | Battino et al. 2019
| M = 4-7 Msun       | [Yields](files/yields_tables/m4m5m6m7_z2m2_Ritter2018.txt)  | -  | Ritter et al. 2018
| M = 12-25 Msun       | [Yields](files/yields_tables/m12m15m20m25_z2m2_z1m2_z6m3_z1m3_z1m4_Ritter1018.txt)  | -  | Ritter et al. 2018
| | | | |
| **Z = 0.01**           |            | |  | 
| M = 1 Msun       | [Yields](files/yields_tables/m1_z1m2_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1z1m2_fin_surfabu.dat)  | Ritter et al. 2018
| M = 1.65 Msun       | [Yields](files/yields_tables/m1p65_z1m2_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1p65z1m2_fin_surfabu.dat)  | Ritter et al. 2018
| M = 2 Msun       | [Yields](files/yields_tables/m2m3_z1m2_z2m2_z3m2_Battino2019.txt) | [Final surface abundances](files/final_surf_abu/m2m3_z3m2_z2m2_z1m2_final_surf_isoabu_Battino2019.txt)  | Battino et al. 2019
| M = 3 Msun       | [Yields](files/yields_tables/m2m3_z1m2_z2m2_z3m2_Battino2019.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z3m2_z2m2_z1m2_final_surf_isoabu_Battino2019.txt)   | Battino et al. 2019
| M = 4-7 Msun       | [Yields](files/yields_tables/m4m5m6m7_z1m2_Ritter2018.txt)  | -  | Ritter et al. 2018
| M = 12-25 Msun       | [Yields](files/yields_tables/m12m15m20m25_z2m2_z1m2_z6m3_z1m3_z1m4_Ritter1018.txt)  | -  | Ritter et al. 2018
| | | | |
| **Z = 0.006**           |            | |  | 
| M = 1 Msun       | [Yields](files/yields_tables/m1_z6m3_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1z6m3_fin_surfabu.dat)  | Ritter et al. 2018
| M = 1.65 Msun       | [Yields](files/yields_tables/m1p65_z6m3_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1p65z6m3_fin_surfabu.dat)  | Ritter et al. 2018
| M = 2 Msun       | [Yields](files/yields_tables/m2_z6m3_Ritter2018.txt) | [Final surface abundances](files/final_surf_abu/m2z6m3_fin_surfabu.dat)  | Ritter et al. 2018
| M = 3 Msun       | [Yields](files/yields_tables/m3_z6m3_Ritter2018.txt) | [Final surface abundances](files/final_surf_abu/m3z6m3_fin_surfabu.dat)  | Ritter et al. 2018
| M = 4-7 Msun       | [Yields](files/yields_tables/m4m5m6m7_z6m3_Ritter2018.txt)  | -  | Ritter et al. 2018
| M = 12-25 Msun       | [Yields](files/yields_tables/m12m15m20m25_z2m2_z1m2_z6m3_z1m3_z1m4_Ritter1018.txt)  | -  | Ritter et al. 2018
| | | | |
| **Z = 0.002**           |            | |  | 
| M = 2 Msun       | [Yields](files/yields_tables/m2m3_z1m3_m2_z2m3_Battino2021.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z1m3_m2_z2m3_final_surf_isoabu_Battino2021.txt)  | Battino et al. 2021
| | | | |
| **Z = 0.001**           |            | |  | 
| M = 1 Msun       | [Yields](files/yields_tables/m1_z1m3_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1z1m3_fin_surfabu.dat)  | Ritter et al. 2018
| M = 1.65 Msun       | [Yields](files/yields_tables/m1p65_z1m3_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1p65z1m3_fin_surfabu.dat)  | Ritter et al. 2018
 M = 2 Msun       | [Yields](files/yields_tables/m2m3_z1m3_m2_z2m3_Battino2021.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z1m3_m2_z2m3_final_surf_isoabu_Battino2021.txt)  | Battino et al. 2021| 
 M = 3 Msun       | [Yields](files/yields_tables/m2m3_z1m3_m2_z2m3_Battino2021.txt)  | [Final surface abundances](files/final_surf_abu/m2m3_z1m3_m2_z2m3_final_surf_isoabu_Battino2021.txt)  | Battino et al. 2021
| M = 4-7 Msun       | [Yields](files/yields_tables/m4m5m6m7_z1m3_Ritter2018.txt)  | -  | Ritter et al. 2018
| M = 12-25 Msun       | [Yields](files/yields_tables/m12m15m20m25_z2m2_z1m2_z6m3_z1m3_z1m4_Ritter1018.txt)  | -  | Ritter et al. 2018
| | | | |
| **Z = 0.0001**           |            | |  | 
| M = 1 Msun       | [Yields](files/yields_tables/m1_z1m4_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1z1m4_fin_surfabu.dat)  | Ritter et al. 2018
| M = 1.65 Msun       | [Yields](files/yields_tables/m1p65_z1m4_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m1p65z1m4_fin_surfabu.dat)  | Ritter et al. 2018
 M = 2 Msun       | [Yields](files/yields_tables/m2_z1m4_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m2z1m4_fin_surfabu.dat)  | Ritter et al. 2018| 
 M = 3 Msun       | [Yields](files/yields_tables/m3_z1m4_Ritter2018.txt)  | [Final surface abundances](files/final_surf_abu/m3z1m4_fin_surfabu.dat)  | Ritter et al. 2018| 
| M = 4-7 Msun       | [Yields](files/yields_tables/m4m5m6m7_z1m4_Ritter2018.txt)  | -  | Ritter et al. 2018
| M = 12-25 Msun       | [Yields](files/yields_tables/m12m15m20m25_z2m2_z1m2_z6m3_z1m3_z1m4_Ritter1018.txt)  | -  | Ritter et al. 2018


## Full detailed stellar structure and nucleosynthesis data
In addition to the recommended dataset above, we also provide the published data associated with each of the publications listed at the top of the page.

| Set1           |            | | 
|----------------|------------|------------|
| Z = 0.02       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1%2Fset1.2%2F)  | [Webpage](https://download1.nugridstars.org/set1/set1.2/)  
| Z = 0.01       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1%2Fset1.1%2F)  | [Webpage](https://download1.nugridstars.org/set1/set1.1/) 
| Yield tables   | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1%2FYield_tables%2F)  | [Webpage](https://download1.nugridstars.org/set1/Yield_tables/)
| Root directory | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1%2F)  | [Webpage](https://download1.nugridstars.org/set1/)

| Set1ext        |            | | 
|----------------|------------|------------|
| Z = 0.02       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2Fset1.2%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/set1.2/)  
| Z = 0.01       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2Fset1.1%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/set1.1/)  
| Z = 0.006      | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2Fset1.3a%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/set1.3a/)  
| Z = 0.001      | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2Fset1.4a%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/set1.4a/)  
| Z = 0.0001     | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2Fset1.5a%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/set1.5a/)  
| Yield tables   | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2FYield_tables%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/Yield_tables/) 
| Root directory | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1ext%2F)  | [Webpage](https://download1.nugridstars.org/set1ext/) 

| Set1upd        |            | |
|----------------|------------|------------|
| Z = 0.03       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.3%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/set1.3/)
| Z = 0.02       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.2%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/set1.2/)
| Z = 0.01       | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.1%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/set1.1/)
| Z = 0.002      | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.02%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/set1.02/)
| Z = 0.001      | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.01%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/set1.01/)
| Yield tables   | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fyields_finalabu_tables%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/yields_finalabu_tables/)
| Root directory | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2F)  | [Webpage](https://download1.nugridstars.org/set1upd/)

**Nomenclature** In each metallicity directory, data are organized as follows.

   Sub-directory | Data
   ----------|------------
  see\_wind  | Stellar evolution output (pre-SN) 
  see\_exp   | Massive star explosion data (delayed and rapid)
  ppd_wind   | Post-processing data of see\_wind
  ppd\_exp   | Post-processing data of see\_exp
  
Sub-directories ending with *yemcut* include data where the remnant mass (mass-cut) of massive star models were defined using the Ye value.

| Project                   | Data Links                                                                                                          |                                                              |
|---------------------------|---------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------|
| super-AGB                 | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2F) | [Webpage](https://download1.nugridstars.org/sagb_jones2016/) |
| Radioactive isotopes ccSN | [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fchetec-infra_models%2FLAW22%2F)                                                                                                          | [Webpage](https://download1.nugridstars.org/chetec-infra_models/LAW22/)                                                  |
|iRAWD| [Globus](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2FiRAWDyields%2F)  | [Webpage](https://download1.nugridstars.org/iRAWDyields)    |  
