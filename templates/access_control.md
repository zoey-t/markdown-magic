We list the privileged roles that have special access to critical functions.

1. `CronusToken.sol`
    - `owner`: mint new tokens.
    - `keeper`: update `maxSupply` limit.
2. `CronusFactory.sol`
    - `feeTo`: the address that can receive the mint fee when the lp token is minted.
    - `feeToSetter`: set `feeTo` and `feeToSetter` address.
3. `MasterChefCronus.sol`
    - `owner` :`add`and `set` pool.
    - `admin`: deposit token for a user.
4. `MoneyMaker.sol`
    - `auth`: authorized address. It can set bridge, dev cut, dev address, `tokenTo` address. It can also convert pairs of tokens to `tokenTo`
    - `owner`: add/remove `auth` role.
5. `StableCronusStaking.sol`
    - `owner`: add/remove reward token and set deposit fee percent.