# clarity-hackathon-stableswap

Steps:
 - follow Hiro guidelines to setup dev environment: https://github.com/hirosystems/clarinet
 - clone repo and cd into the clarity-hackathon-stableswap directory
 - run clarinet console to test functions. examples below:
    - create-pair:
        (contract-call? .stableswap-v2 create-pair .usda-token .xusd-token "usda-xusd" u500000 u500000)
        
    - add-to-position:
        (contract-call? .stableswap-v2 add-to-position .usda-token .xusd-token u500000 u500000)    
        
    - reduce-position:
        (contract-call? .stableswap-v2 reduce-position .usda-token .xusd-token u10)
        
    - create-pair:
        (contract-call? .stableswap-v2 swap-x-for-y .usda-token .xusd-token u25000 u25000)       
