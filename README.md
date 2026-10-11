# Polymarket Session Keys Guide

A practical guide to scoped signers (Session Keys) on Polymarket - why your trading key should never be your storage key.

By [Srey Leak](https://github.com/sreyleak-security) - security researcher, ex-Coinbase security engineering. Long Beach, CA.

## The one-sentence version

Sign trades with a limited, expiring key - keep your master key cold and boring.

## Why most traders get this wrong

The default is convenient: one key signs everything. Convenience is exactly what attackers rely on. At Coinbase, nearly every account-takeover incident started with a hot key that had too much power.

## The three rules

1. **Separation.** Trading key is not storage key. Ever.
2. 2. **Scoping.** The daily signer holds only what you can afford to lose this week.
   3. 3. **Expiry.** Sessions expire in days. Renewing deliberately is a feature, not a chore.
     
      4. ## What's in this guide
     
      5. - docs/setup-walkthrough.md - step-by-step Session Key setup (coming)
         - - docs/threat-model.md - what a compromised signer can and cannot do (coming)
           - - examples/ - minimal config examples (coming)
            
             - ## Related
            
             - - [polymarket-security-checklist](https://github.com/sreyleak-security/polymarket-security-checklist) - the full pre/during/post-trading checklists
              
               - ## Disclaimer
              
               - Educational content only. Not financial advice. Not official Polymarket documentation.
               - 
