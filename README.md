# clarity-hackathon-stableswap

Steps:
 - follow Hiro guidelines to setup dev environment: https://github.com/hirosystems/clarinet
 - clone repo and cd into the clarity-hackathon-stableswap directory
 - run clarinet console to test functions. 
 
 
 - public function examples:
    - create-pair:
        (contract-call? .stableswap-v2 create-pair .usda-token .xusd-token "usda-xusd" u500000 u500000)
        
    - add-to-position:
        (contract-call? .stableswap-v2 add-to-position .usda-token .xusd-token u500000 u500000)    
        
   - swap-x-for-y:
        (contract-call? .stableswap-v2 swap-x-for-y .usda-token .xusd-token u25000 u25000)            
   
   - reduce-position:
        (contract-call? .stableswap-v2 reduce-position .usda-token .xusd-token u10)
        


 - read-only function examples:
    - get-name (of pair in stable swap pool):
        (contract-call? .stableswap-v2 get-name .usda-token .xusd-token)
        
    - get-balances (of tokens in the stableswap pool):
        (contract-call? .stableswap-v2 get-balances .usda-token .xusd-token)    
        
