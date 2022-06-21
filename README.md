# Criacao-Token-Solana
Criacao de um token na solana

Os passos para criacao de uma conta para uso sao os seguintes:

solana config set --url https://api.devnet.solana.com

solana-keygen grind --starts-with Tok:1

solana config set --keypair (Tokaskdjahskdhas.json arquivo.json criado no comando acima)

solana airdrop 2

#Agora vamos para criacao do token SPL

spl-token create-token

spl-token create-account (codigo do token criado no comando acima: C3nZ6813otSJHSdjshdJHDTFsvAnTe1ngQ5vHnneBo)

spl-token mint (codigo do token criado) 1000 (1000 no caso é a quantidade de tokens que quer q seja criado, nesse caso 1000 tokens)

para checar o supply: spl-token supply (codigo do token criado)

Para transferir o token criado para uma outra conta:

spl-token transfer (codigo do token criado) 50 (codigo da carteira para onde vai enviar o token) --fund-recipient


#####################

Veja esse tutorial para criar o Nome e o Logo do Token na rede da solana atraves do Fork e PR no Github.

https://learn.figment.io/tutorials/sol-mint-token
