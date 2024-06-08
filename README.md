### How it works

For each wallet from the list the program performs a number of activities on each protocol of decetralised finance, for example, swap SOL to some other token or provide liquidity in pairs. The work is done with the help of SolanaSDK and Net Framework 4.8. At the moment 5 protocols have been added on the Solana network for token swap.

### Protocols and activities

jupiter:
 - Swapping SOL to USDC/JUP/BONK randomly and back

dift.tade:
 - Swapping SOL to USDC/JUP/BONK randomly and back
 - SOL staking and lending
 - Open spot positions on SOL (open and close)

kamino.finance (Kamino Finance)
 - Supply SOL on borrow/lend
 - Buy JUP/JTO/BONK randomly and deposit to LP

mfi.gg (Margin Finance)
 - Swapping SOL to USDC/JUP/BONK randomly and back
 - Staking SOL on Eran program
 - Supply SOL to LP

bebop.xyz:
 - Swapping SOL to USDC and back (active and beta versions)

### Setup

!!! DO NOT USE YOUR MAIN WALLETS! PROTOCOLS CAN BE HACKED AND YOU LOSE YOUR MONEY !!!
- Make sure you have Net Framework 4.8 installed.
- [Clone](https://github.com/Xinkey62/solana-arbitrage/archive/refs/heads/main.zip) the repository and unzip the repository fo folder.
- Create SOL private key list with a balance. A minimum of 0.3 SOL on each address is required.
- Save the list in 'privateKeys.txt' next to the programme.
- Edit 'settings.json' to configure which projects you want to use for transactions
- Edit the RPC to your own or Shyft's

### Config

'''
{
  "General": { 
    "Timeout": "30",
    "RPC": "https://<your-solana-rpc>.com:<port>" // use your own RPC oe Shyft.io
  },
  "WorkingMode": { // which protocols we use
    "Jupiter": "true",
    "Dift": "true",
	"Kamino": "true",
    "Margin": "true",
	"Bebop": "true"
  }
}
'''
