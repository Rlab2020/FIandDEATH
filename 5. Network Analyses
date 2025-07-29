## proteins = column names of proteins



library(WGCNA)



## CHOSE POWER
powers = c(c(1:20), seq(from = 22, to=30, by=2))
sft = pickSoftThreshold(datExpr, powerVector = powers, verbose = 5)
power <- sft$powerEstimate

## RUN WGCNA
cor <- WGCNA::cor
net <- blockwiseModules(datExpr, power = power,
                       TOMType = "signed", minModuleSize = 10,
                       reassignThreshold = 0, mergeCutHeight = 0.25,
                       numericLabels = TRUE, pamRespectsDendro = FALSE,
                       saveTOMs = F,
                       verbose = 3)

# The network analysis for identified proteins were performed by running the above code.
