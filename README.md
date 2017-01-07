Using OFX via the net, the goal is to retrieve as much info as possible via
cli.

To use this, you will need to obtain info about your financial institution,
and plug the bits into 'ofxcli.conf' to be installed as $HOME/.ofxcli.conf.

Example output:

```
t0|todd@i5/pf ~/git/sw/ofxcli|3981$ ./ofxcli
ORG: Organization Name
FID: 123456789
URL: https://ofx.examplebank.com/OFX/ofx.html
Seems ok so far:
Signon status code: 0
    Account Available    Ledger
     Number   Balance   Balance     Type Name
   12345678      0.02      0.02  SAVINGS Test Savings Account
```

Ultimately, this will permit repackaging the info into files for various
accounting software that may not have native OFX support, e.g. ledger.
