## list = a  vector containing identified proteins



library(clusterProfiler);library(org.Hs.eg.db)



## ENRICHMENT ANALYSIS OF GO
go <- enrichGO(list,
               OrgDb = org.Hs.eg.db,
               ont='ALL',
               pAdjustMethod = 'BH',
               pvalueCutoff = 1,
               qvalueCutoff = 1,
               keyType = 'ENTREZID',
               readable = T
)

# The enrichment analysis of GO terms for identified proteins were performed by running the above code.



## ENRICHMENT ANALYSIS OF KEGG
kegg <- enrichKEGG(list, 
                   organism = 'hsa',
                   keyType = 'kegg',
                   pvalueCutoff = 1,
                   qvalueCutoff = 1,
                   pAdjustMethod = 'BH',
                   use_internal_data = F
)

# The enrichment analysis of KEGG pathway for identified proteins were performed by running the above code.
