# stkd-SCRT Staking Derivative Constitution
## What is stkd-SCRT?

stkd-SCRT is a Shade Protocol staking derivative that represents staked SCRT on Secret Network, combining the cumulative value of deposited SCRT collateral with compounded staking rewards via the staking derivative contract. stkd-SCRT tokens are minted via deposits of SCRT.

When stkd-SCRT are redeemed, they are burned in return for the originally deposited SCRT and respective accumulated staking rewards after a 21 day unbonding period. When stkd-SCRT is minted or burned, a fee goes directly to the ShadeDAO — creating a revenue stream for SHD holders.

## Validator Set
The stkd-SCRT contract automatically stakes the SCRT that users deposit when minting stkd-SCRT. This staked amount is divided between a set of validators at specific wights as programmed into the contract. This validator set and/or weights can be modified by the administrator of the contract. 

## Contract Administrator
At the launch of stkd-SCRT, the contract will be administered by a multi-sig wallet controlled by core developers of Shade Protocol. Once Shade Protocol has completed the development of its governance module, the control of the stkd-SCRT contract will be handed over to the ShadeDAO to be run by the Shade community.

## Validator Selection
We hope that by outlining the requirements to join the validator set we can create transparency and foster inclusion. Exclusion from the list is not permanent and validators should be able to understand how they can be included in the next update. The barrier to entry may require validators to compromise on fees, to participate in governance, or to make their infrastructure more robust. These rules reflect a balance that we feel is best for the product and the network.


| Rule                                | Type         | Reason                            |
|-------------------------------------|--------------|-----------------------------------|
| No Exchange Validators              | Qualitative  | Increase Network Decentralization |
| No 0% Validator in Top 20           | Quantitative | Increase Network Decentralization |
| Reasonable Gas Fee (<=0.0125 uSCRT) | Quantitative | Network Usability                 |
| Participation in 66.6% of Gov Props | Quantitative | Network Sustainability            |
| Uptime > 97.5%                      | Quantitative | Product/Network Sustainability    |
| Top 66.6% of Nodes in Uptime        | Quantitative | Product/Network Sustainability    |
| Top 80% of Nodes in SCRT Staked     | Quantitative | Product Sustainability            |
| Current Maximum Commission <= 5%     | Quantitative | Product Sustainability            |
| Maximum Commission Validator <=20%   | Quantitative | Product Sustainability            |
| Daily Max Commission Change <=1%     | Quantitative | Product Sustainability            |


### No Exchange Validators
- Exchanges as an entity are already staking their users coins on their behalf. To increase decentralization we believe that we should not contribute to this process. Exchange nodes do not pay the entirety of the staking commission to their users, but keep a large portion for themselves. 

### No 0% Validator in Top 20
- This provides a clear break on where a node is using 0% validator fees to get increased delegations may begin to hurt the rest of the chain. We believe that some floor of commission fee should be set at a certain point. Users who want to continue staking with 0% fees can redelegate down the list and increase decentralization.

### Reasonable Gas Fee
- In the past we’ve seen validators that while producing blocks, do not validate transactions. This led to higher fees, as well as failed transactions. With the recent upgrade it’s no longer as much of an issue, but something to keep an eye on.

### Participation in 66.6% of Gov Props
- We believe that validators should be rewarded for the effort they put into the chain. Validators who stay current on their voting (even if it’s an abstain) show a level of dedication to the SCRT ecosystem. This will be judged on the past quarter’s governance props.

### Uptime >97.5%
- This is an important feature for the product and the network’s sustainability. To generate staking rewards the nodes must show an acceptable level of ability in producing blocks. This helps ensure the stability of the network and the staking reward’s of the product's users. This will be judged on the past quarter’s performance.

### Top 66.6% of Nodes by Uptime %
- This is an important feature for the product and the network’s sustainability. To generate staking rewards the nodes must show an acceptable level of ability in producing blocks. It also creates an environment of performance which rewards the best performing node-runners. The purpose of this is to encourage nodes to always search for how to improve their capabilities, not reach a minimum requirement. 

### Top 80% of Nodes by SCRT Staked
- This is an important feature for the product’s sustainability. The node should be an ongoing concern and have enough delegations that it can survive on its own. In the case of it falling out of the active validator set the product would lose staking revenue.

### Current Maximum Commission <=5%
- This an important feature for the product’s sustainability. The fees when staked in the derivative contract should not be higher than the fees users typically bond at. The contract itself has a fee that’s the weighted average of the validators it is staked to. This ensures that the commission remains within a standard range. 

### Maximum Commission Validator <=20%/Daily Max Commission Change <=1%
- This is an important feature for the product’s sustainability. Since the selection is done manually and not via a smart contract we believe any changes to these parameters default settings are considered higher risk for required action in the middle of the quarterly process.

## Validators List
This is the validator list that met the criteria in Q1 2022

| Validator                           |  weight |
|-------------------------------------|---------|
| 🪐 𝕊ecret 𝕊aturn / 1% forever       | 4.61%   |
| SecretChainGirl Capital             | 4.61%   |
| playalongs                          | 4.61%   |
| securesecrets.org                   | 9.00%   |
| 𝕊hadowRealm                         | 4.61%   |
| XavierCapital                        | 4.61%   |
| Ronin Ventures                      | 4.61%   |
| BlockNgine 🛡 Slash Protected       | 4.61%   |
| 0% Fee to 2023 / Stakewolle.com      | 4.61%   |
| Lavender.Five Nodes 🐝               | 4.61%   |
| Smart Stake - 0% till Apr 2022     | 4.61%   |
| DomeriumLabs                       | 4.61%   |
| secretSauce 🍯                     | 4.61%   |
| Order of Secrets / 1% fees          | 4.61%   |
| secretnodes.com                     | 4.61%   |
| Mario                               | 4.61%   |
| WhisperNode                         | 4.61%   |
| Trivium / Trivium.Network           | 4.61%   |
| Secret Keeper                      | 4.61%   |
| Mr Roboto                           | 4.01%   |
| Stake or Die                        | 4.01%   |


- Secure Secrets has the highest weighting in the validator set due to (1) running the bot that spends SCRT as gas to auto-compound staking rewards for all stkd-SCRT holders (2) primary developer group growing the product.
- Mr. Roboto & StakeorDie are also included as core developers of stkd-SCRT, but at a lower weight due to not meeting all the rules outlined above. 
  
## Validator Change Process

- The ShadeDAO governance will control the validator change process, however while Shade Protocol governance is still in development, the change process will be owned by trusted community members of Secret Network. 
- The change process will initially be led by Pmuecke who is the lead of Secret Network’s governance committee. 
- The goal is to make this an impartial process neutral to politics. 

### Change Frequency
- Validator review will be completed at the beginning of each quarter.
- Queries will be performed on a regular basis to understand the uptime of each node. This information will be aggregated to rank validator performance and apply any rules related to this measure outlined above. Validators will be penalized for lack of information, implying one full period of performance is required to be included.


## stkd-SCRT Fees
- A 1% fee is charged for minting stkd-SCRT from SCRT deposits. 
- A 1% fee is charged for withdrawing stkd-SCRT to convert back to SCRT. 
- The stdk-SCRT validator set is NOT the collector of fees.
- These fees are collected by the ShadeDAO.
- The ShadeDAO will control changes to the fee rate. No changes shall be made to the fees until the ShadeDAO has full control as administrator of the stkd-SCRT contract.

## Constitution Amendment Process
- The ShadeDAO governance will control how amendments are made to this constitution.
- While Shade Protocol governance is still in development, the change process will be owned by the same community members that review the validator set as described in the Validator Change Process section above.  

## Constitution Amendment History

Github change history can be viewed to see changes to this document. The table below will also be updated for reference.

| Amendment Number | Description                   |  date     |
|----|---------------------------------------------|-----------|
| 1.1  | This is an example amendment description. Referencing public discussions such as a forum thread is recommended.   | 3/24/2022 |

(Amendment #1.1 is just an example and should be modified whenever a real amendment is put in place)