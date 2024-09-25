# Smart Contract - Starknet
A project in Cairo language that develops a basic Smart Contract on Starknet, with functions to view and increase balance, ideal for new developers.

# Infrastructure
- scarb 2.6.5
- starkli 0.3.4
- starknet-devnet 0.1.2

# Variables 
- Create the keystore ".c-wallets/keystore.json"
- Create the conta ".c-wallets/account.json"
- RPC "http://127.0.0.1:5050"

# Tests
- First we use the command to read, change the contract:
  "starkli call --rpc http://127.0.0.1:5050 0x078d65e4aacecdaa8debc745825a4b4e1711098cfd7584d09917e8e771fb665a get_contador"
- Returns:
  "0x0000000000000000000000000000000000000000000000000000000000000012"
- Then we use the other command, which adds 1 to the contract value:
  "starkli invoke --rpc http://127.0.0.1:5050 --account .c-wallets/account.json --keystore .c-wallets/keystore.json 0x078d65e4aacecdaa8debc745825a4b4e1711098cfd7584d09917e8e771fb665a increase
_contador"
- After the above step, when repeating the command:
  "starkli call --rpc http://127.0.0.1:5050 0x078d65e4aacecdaa8debc745825a4b4e1711098cfd7584d09917e8e771fb665a get_contador"
- This returns us:
  "0x0000000000000000000000000000000000000000000000000000000000000013"

# Prints

![11](https://github.com/user-attachments/assets/ce6137c3-0c7b-4199-9346-389c60409f8f)
![22](https://github.com/user-attachments/assets/a07654de-fb1e-42d8-bd44-b1a3021f22e3)
![2](https://github.com/user-attachments/assets/d7ca06ae-d5a0-4202-9c0e-1dacb98cb53a)


