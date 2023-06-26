# Data and code for: Growth-defence trade-offs facilitate species coexistence in recently diverged spiral gingers.
---

Abstract:
Trade-offs are crucial for species divergence and coexistence. Trade-offs between investment in growth versus defence against herbivores have been implicated in tropical plant species' coexistence. However, the role of growth-defence trade-offs in the coexistence of closely-related species has yet to be explored empirically. Costus villosissimus and C. allenii are recently diverged, interfertile species primarily isolated by adaptation to divergent habitats. Their divergent adaptation involves differences in growth rate, suggesting that trade-offs result in different levels of herbivore defence. Here we ask how differences in herbivore defence are involved in the divergent habitat adaptation that isolates these species. We characterise differences in leaf toughness and chemistry, investigate natural patterns of herbivory, and evaluate the feeding preferences of primary beetle herbivores in controlled trials and field-based experimental arrays. We find clear trade-offs in growth and defence: slower-growing C. allenii has tougher leaves and higher defence chemical concentrations than faster-growing C. villosissimus. However, patterns of wild herbivory do not correspond to differences in defence but instead correspond to specialist herbivore habitat preference. We find that biotic and abiotic selection pressures act via growth-defence trade-offs to promote divergent habitat adaptation key to species maintenance between these close relatives.

## Description of the data and file structure

Here, we outline the data files used in the article described above. 

# rainfall
Gamboa_ra.csv - Rainfall data for Gamboa, Panama from the Panama Canal Authority (ACP). The 'ra' column gives the amount of rain that fell in that ~5min interval. 
# map figure
envs.tif - climate raster stack; created using getclimateraster.R; stacked in this order: bio1,bio4,bio12,bio15
cleaned.occurrences.csv - Costus occurance data from Vargas et al. 2020
julia_pairs.csv - Basic relationship data for the clade of 4 species plotted. 
# leaf toughness
leaf.toughness.csv - Contains 3 leaf toughness measures per individual, taken at 3 locations on the leaf, and the avarage for the leaf/plant. 
# leaf chemistry
Full_chem_data.csv - Chemistry data for 6 individuals of each species.
# wild herbivory data 
vill-all_RLB-herbivory_data_2019-Herbivory.csv - Percent herbivory data for all plants measured in 2019.
2022_wild_herbivory.csv - Percent herbivory data for all plants measured in 2022
# beetle feeding trials
beetle_trials.csv - Data from beetle feeding trials. The beetle choice trials analyzed for this article are those with "alle/vill" in the "Species.in.trial" column. Other rows have palatability data from trials in which beetles only had one leaf square of one species to eat. Analysis of this data was removed from the article as there are not enough trials to overcome huge variability in individual beetle "hungriness". We were able to account for this by calculating a preference score from the choice trials. 
# herbivory arrays
Herbivory_arrays_220703.csv - Data from experimental herbivory arrays placed in the field, in beetle favorable habitat. This file was only used for the herbivory_yn column, not for the percent herbivory data.
array_subset_all_ests.csv - Percent herbivory data from the subset of arrays where we could get estimates of herbivory area. 

## Code/Software

GDTO_analyses.qmd - Quarto markdown of analyses and figure building code written in R 4.2.3
