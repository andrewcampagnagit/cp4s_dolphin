# cp4s_dolphin
Dolphin deployment for CP4S

---

#### Steps to deploy Cloud Pak for Security

1. Download dolphin onto target installation machine

**Note:** Only use beta-4 release of dolphin or higher only for ConfigBlock & OpenShiftBlock processors and multi-mode processor selection support.

https://github.com/andrewcampagnagit/dolphin

2. Ensure you have tls.crt, tls.key, and ca.crt certificates available on deployment machine

Utilize OpenSSL and reference the [IBM Knowledge Center](https://www.ibm.com/docs/en/cloud-paks/cp-security/1.7.0?topic=planning-domain-name-tls-certificates) to create these certificates

3. Run dolphin deployment

```bash
dolphin deploy -mG https://raw.githubusercontent.com/andrewcampagnagit/cp4s_dolphin/main/manifest.json
```

4. Follow the prompts

The deployment has a series of prompts asking for entitlement key, FQDN, certificates, etc. All prompts will include a link to the IBM Knowledge Center on how to acquire each required value.

#### Verification

Test blocks are included in the **instructions.json** which simply verify all **iscsequence** are in the Successful state.

