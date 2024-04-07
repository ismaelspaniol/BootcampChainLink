Avalanche Fuji - setup
Origem Blockchain
Avalanche Fuji

Destino Blockchain
Ethereum Sepolia

Adicionar Fuji em Metamask
https://chainlist.org/chain/43113

Connect wallet
Avalanche Fuji Testnet - Add to Metamask
Confirmar no Metamask

Faucet
Get Avax Fuji and LINK on Fuji
https://workshop-faucet.vercel.app/faucets/fuji
Senha: LinkShadowFork18


Depois da aula
LINK e Avax Fuji
https://faucets.chain.link/

Avax Fuji
https://www.allthatnode.com/faucet/avalanche.dsrv

LINK em Fuji em Metamask
https://docs.chain.link/resources/link-token-contracts#fuji-testnet

Avax Fuji Block explorer
https://testnet.snowtrace.io/

USDC
Add to Metamask
How to import USDC to your Metamask wallet
https://developers.circle.com/stablecoins/docs/usdc-on-test-networks

USDC address - Avalanche Fuji testnet
0x5425890298aed601595a70ab815c96711a31bc65
https://testnet.snowtrace.io/token/0x5425890298aed601595a70ab815c96711a31bc65


Faucet - USDC from Avalanche Fuji testnet
https://faucet.circle.com/
Seleciona Avalanche Fuji testnet
Endereço da sua carteira

Outro faucet com USDC en Avalanche Fuji
https://core.app/tools/testnet-faucet/?subnet=c&token=usdcc

Referencias - USDC
https://learn.circle.com/quickstarts/cctp
https://developers.circle.com/

************************************
Remix
https://remix.ethereum.org/

Icon 5 - DEPLOY & RUN TRANSACTIONS
ENVIRONMENT
Injected provider - Metamask
Check if you are on Custom (43113) network = Fuji

TransferUSDCBasic
Icon 2 - FILE EXPLORER

File: 
TransferUSDCBasic.sol

Deploy










Approve USDC = Aprovar seu contrato a usar USDC da sua carteira Metamask
usdcAmount: 1 USDC
1000000

Approve - no Remix

Icon 5 - DEPLOY & RUN TRANSACTIONS
Contract - selecionar
IERC20
NAO faz deploy!
At Address
Parametro:
0x5425890298aed601595a70ab815c96711a31bc65
(USDC address)
Clica no botao At Address

Vai para baixo - Deployed/Unpinned Contracts

Expande IERC20

Expande Approve
spender (address): endereco do seu smart contract

value (uint256): 1000000
1 USDC
Clica Transact


Va para o seu smart contract

Execute
allowanceUsdc

O resultado deve ser
0:uint256: usdcAmount 1000000


Enviar LINK para o contrato, para pagar as fees
No Metamask
Tokens => LINK => Send
Envia 3 LINK para o endereco do seu smart contract

No smart contract

BalancesOf
Parametro: Endereco do smart contract

Resultado
0:uint256: linkBalance 3000000000000000000
1:uint256: usdcBalance 0


Verifique se esta tudo pronto!

allowanceUsdc: 
0:uint256: usdcAmount 1000000

BalancesOf (Parametro: Endereco do smart contract)
0:uint256: linkBalance 3000000000000000000
1:uint256: usdcBalance 0

transferUsdcToSepolia
_receiver: Endereco da sua carteira no Metamask
_amount: 1000000
= 1 USDC

Clica en Transact

CCIP Explorer
https://ccip.chain.link/


************************************
USDC em Sepolia
Em Metamask
Selecionar Sepolia

Add token USDC em Sepolia
Tokens => Import Token
0x1c7D4B196Cb0C7B01d743Fbc6116a902379C7238
https://sepolia.etherscan.io/address/0x1c7D4B196Cb0C7B01d743Fbc6116a902379C7238 











