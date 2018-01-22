# Business Network Definition
# SFD Sistema Financeiro Digital

## HyperLedger Composer Implementation for SFD
* Composer Version 0.16.3
* Fabric Version 1.0

## Model Files

* assets.cto
    ContaIF - Financial Institution account
    Cliente - The End User that requests funds transfer

* participant.cto
    InstituicaoFinanceira - the Financial Institution
    BancoCentral - The Central Bank

* transactions.cto
    EmiteDDR - cash-in to central bank account
    RecolheDDR - cash-out from central bank account
    Pledge - funds transfer from central bank account to financial institution account
    Redeem - funds transfer from financial institution account to central bank account
    TransferenciaFundos - funds transfer between two IFs accounts

* events.cto
    PledgeEvent
    RedeemEvent
    TransferenciaFundosEvent

## Script Files

* bc.js     - Central Bank Transactions Scripts
* cliente.js - Cliente Transactions Scripts
* if.js - Financial Institution Transactions Scripts
