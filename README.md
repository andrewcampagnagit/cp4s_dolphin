# cp4s_dolphin
Dolphin deployment for CP4S

#### Steps to deploy Cloud Pak for Security

1. Download dolphin onto target installation machine

https://github.com/andrewcampagnagit/dolphin

2. Run dolphin deployment

```bash
dolphin deploy -mG https://raw.github.ibm.com/Andrew-Campagna/cp4s_dolphin/master/manifest.json?token=AACDEXJ3DA2OMDYDES55KITAIBZ24
```

#### Verification

Test blocks are included in the **instructions.json** which simply verify all **iscsequence** are in the Successful state.

