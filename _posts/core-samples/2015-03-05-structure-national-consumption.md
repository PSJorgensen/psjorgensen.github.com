{% include JB/setup %}

    # READING IN DATA
    ## SETTING DIRECTORY FOR EORA DATA ON LOCAL HARD DRIVE
    wd<-"G:/Documents/PostDocKVA/Data/Eora" ### data directory
    setwd(wd)
    dir()

    ##  [1] "countries.csv"              "country_lookup.csv"        
    ##  [3] "Eora26_2011_bp.zip"         "Eora26Structure.xlsx"      
    ##  [5] "gdppop.csv"                 "regionmembership.csv"      
    ##  [7] "TradeBalance_I-ENERGY.csv"  "TradeBalance_I-ENERGY.xlsx"
    ##  [9] "TradeBalance_I-VA.csv"      "TradeBalance_I-VA.xlsx"    
    ## [11] "Wiedmann"

    ## READING IN MATERIAL USE DATA
    wd<-"G:/Documents/PostDocKVA/Data/Eora" ### data directory
    setwd(wd)
    dir()

    ##  [1] "countries.csv"              "country_lookup.csv"        
    ##  [3] "Eora26_2011_bp.zip"         "Eora26Structure.xlsx"      
    ##  [5] "gdppop.csv"                 "regionmembership.csv"      
    ##  [7] "TradeBalance_I-ENERGY.csv"  "TradeBalance_I-ENERGY.xlsx"
    ##  [9] "TradeBalance_I-VA.csv"      "TradeBalance_I-VA.xlsx"    
    ## [11] "Wiedmann"

    energy.df<-read.csv("TradeBalance_I-ENERGY.csv",header=TRUE)
    head(energy.df)

    ##       Country CountryA3    y TerritorialEmissions Imports Exports
    ## 1 Afghanistan       AFG 2011                 2120   47872      32
    ## 2     Albania       ALB 2011                76785   38725    8777
    ## 3     Algeria       DZA 2011              1595798  275304  791087
    ## 4     Andorra       AND 2011                    0    8185       0
    ## 5      Angola       AGO 2011               568776  174772  120704
    ## 6     Antigua       ATG 2011                    0    7192       0
    ##   DirectEmissions Consumption
    ## 1             949       49959
    ## 2           11011      106734
    ## 3          251668     1080016
    ## 4               0        8185
    ## 5          255897      622844
    ## 6               0        7192
