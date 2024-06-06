---
permalink: /markdown/
title: "Modification of a Multi-party Computation Protocol"
author_profile: true
redirect_from: 
  - /md/
  - /markdown.html
---
<!-- ## Modification of a Multi-party Computation Protocol -->
* The MPC protocol of [Fluid MPC](https://eprint.iacr.org/2020/754) operates under a dynamic but synchronous model. However, some participants may experience poor network conditions or even disconnections. Thus, it is more realistic to consider an asynchronous environment. We aim to modify this protocol so that it can be effectively used in such settings.

* We follow the work of [Fluid MPC](https://eprint.iacr.org/2020/754) and [HoneyBadgerMPC](https://eprint.iacr.org/2019/883). 

* I was responsible for part of the [implementation codes](https://github.com/HTseaaat/admpc_htadkg).

![MPC Protocol Diagram](/files/Project_ADMPC.png)

# Blockchain wallets based on efficient lattice signature

* We follow the work of [Musig-L](https://eprint.iacr.org/2022/1036), modified this signature and found an application of it.

* We add a randomness to the online phase, thus every participant will compute several online threads and the first one thhat passes through the rejection sampling is output as the final result. 

![Protocol Modification](/files/Project_Musig_L.png)

* I was responsible for part of the [implemention code](https://github.com/BBINGWU/MuLPay-CISCN).
