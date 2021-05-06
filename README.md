# cp4s_dolphin
Dolphin deployment for CP4S

#### Steps to deploy Cloud Pak for Security

1. Download dolphin onto target installation machine

**Note:** Only use beta-4 release of dolphin or higher only for ConfigBlock & OpenShiftBlock processors and multi-mode processor selection support.

https://github.com/andrewcampagnagit/dolphin

2. Run dolphin deployment

```bash
dolphin deploy -mG https://raw.githubusercontent.com/andrewcampagnagit/cp4s_dolphin/main/manifest.json
```

#### Verification

Test blocks are included in the **instructions.json** which simply verify all **iscsequence** are in the Successful state.

