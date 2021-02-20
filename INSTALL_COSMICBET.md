# Install casino 

## Download `cosmic-devnet-2`

```
git clone https://github.com/cosmicbet/ledger
cd ledger && git checkout -t origin/riccardo/wta && make install
```

## Install
## inserire comandi wget genesi, sed per peers e provare....in aggiornamento

```

casino start --pruning=nothing > ~/casinod.log 2>&1 &
```


 casinod tx staking create-validator --amount=1000000ufchs --moniker=$VALIDATOR_NAME --from=$WALLET_NAME --pubkey=$(casinod tendermint show-validator) --commission-max-rate="0.20" --commission-max-change-rate="0.01" --min-self-delegation="1" --gas="auto" --commission-rate="0.10" --commission-max-change-rate="0.5" --commission-max-change-rate="0.2" --chain-id="cosmic-devnet-2"
