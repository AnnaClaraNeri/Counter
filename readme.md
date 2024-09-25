# Smart Contract - Starknet
A project in Cairo language that develops a basic Smart Contract on Starknet, with functions to view and increase balance, ideal for new developers.

# Infrastructure
- scarb 2.6.5
- starkli 0.3.4
- starknet-devnet 0.1.2

# Variables 
- Create the keystore: ".c-wallets/keystore.json"
- Create the conta: ".c-wallets/account.json"
- RPC: "http://127.0.0.1:5050"

# Tests
- First we use the command to read, change the contract:
  
-"starkli call --rpc http://127.0.0.1:5050 0x078d65e4aacecdaa8debc745825a4b4e1711098cfd7584d09917e8e771fb665a get_contador"
  
- Returns:
  
-"0x0000000000000000000000000000000000000000000000000000000000000012"
  
- Then we use the other command, which adds 1 to the contract value:
  
-"starkli invoke --rpc http://127.0.0.1:5050 --account .c-wallets/account.json --keystore .c-wallets/keystore.json 0x078d65e4aacecdaa8debc745825a4b4e1711098cfd7584d09917e8e771fb665a increase_contador"
  
- After the above step, when repeating the command:
  
-"starkli call --rpc http://127.0.0.1:5050 0x078d65e4aacecdaa8debc745825a4b4e1711098cfd7584d09917e8e771fb665a get_contador"
  
- This returns us:
  
-"0x0000000000000000000000000000000000000000000000000000000000000013"

# Prints

![01](https://github.com/user-attachments/assets/7fbc8c44-6258-4129-9420-4efdcf0310a0)
![02](https://github.com/user-attachments/assets/3076e580-aa7d-4627-bbfe-2eea25033b5e)
![03](https://github.com/user-attachments/assets/7a0dc03e-f38a-47b4-b195-ffa7dac13f1f)





