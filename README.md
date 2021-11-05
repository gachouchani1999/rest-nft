# REST NFT
An extended CW721 (v0.9.2) with update, burn, freeze, set_minter functionalities.

## Methods
1. `burn`
    Destroys a token, decreasing token count.
    ```
    Burn {
        token_id: String,
    }
    ```
2. `update`
   ```
    Update {
        token_id: String,
        token_uri: Option<String>,
        metadata: Extension,
    }
   ```
3. `freeze`
   Freezes changes to all token metadata.
   ```
   Freeze {}
   ```
4. `set_minter`
    Current minter can transfer minter rights to others.
    ```
    SetMinter {
        minter: String,
    }
    ```

## Usage

Contracts are used for by all REST-verse NFTs (tadpoles, toads).
It supports a mint, burn, update and freeze launch mechanic.
