This wiki includes the list of Linux kernel patches that have been merged, or are in review on the public mailing list (i.e. LKML) to support Intel base TDX. 
# Host
## Merged patches
| Patch description | Kernel version | Lore link | Category | Commit ID |
|-------------------|----------------|-----------|----------|-----------|
| KVM HW enable/disable | v6.3 | https://lore.kernel.org/lkml/20221130230934.1014142-1-seanjc@google.com/ | boot | 2b01281273738bf2d6551da48d65db2df3f28998..9f1a4c004869d3c8061f286fec4d8096dd099b84 |
| Unify TDCALL/SEAMCALL and TDVMCALL assembly | v6.7-rc1 | https://lore.kernel.org/lkml/cover.1692096753.git.kai.huang@intel.com/ | boot | 5d092b66119d774853cc9308522620299048a662..7b804135d4d1f0a2b9dda69c6303d3f2dcbe9d37 |
| TDX host kernel support | v6.8-rc1 | https://lore.kernel.org/lkml/cover.1699527082.git.kai.huang@intel.com/ | boot | 765a0542fdc7aad7cbc1da3bd19bed6297b54e2c..4e1c7dddc71708c21d7fe69cc5f8297ffb7c6965 |
| KVM: guest_memfd() and per-page attributes | v6.8-rc1 | https://lore.kernel.org/lkml/20231105163040.14904-1-pbonzini@redhat.com/ | boot | e97b39c5c4362dc1cbc37a563ddac313b96c84f3..5d74316466f4aabdd2ee1e33b45e4933c9bc3ea1 |
## Patches in review
| Patch description | patch version | Lore link | Category |
|-------------------|---------------|-----------|----------|
| KVM TDX basic feature support | v18 | https://lore.kernel.org/all/cover.1705965634.git.isaku.yamahata@intel.com/ | boot |
| KVM TDX: TDP MMU: large page support | v7 | https://lore.kernel.org/lkml/cover.1705965958.git.isaku.yamahata@intel.com/ | performance |
| x86/mce, KVM: X86: KVM memory poison and MCE injector support | v1 | https://lore.kernel.org/all/cover.1696926843.git.isaku.yamahata@intel.com/ | integrity |
| tsm: Runtime measurement registers ABI | v2 | https://lore.kernel.org/all/20240128212532.2754325-1-sameo@rivosinc.com/ | attestation |

# Guest
## Merged patches
| Patch description | Kernel version | Lore link | Category | Commit ID |
|-------------------|----------------|-----------|----------|-----------|
| Confidential shared infrastructure | v5.16 | https://lore.kernel.org/lkml/20210928191009.32551-1-bp@alien8.de/ | boot | 402fe0cb71032c4bc931ac70a6b024408e09f817..e9d1d2bb75b2d5d4b426769c5aae0ce8cef3558f |
| Extend confidential computing API | v5.18 | https://lore.kernel.org/all/20220222185740.26228-1-kirill.shutemov@linux.intel.com/ | boot | 655a0fa34b4f7ac6e2b1406fab15e52a7b6accb1..1e8c5971c249893ac33ca983c32bafcf5d50c727 |
| TDX preparation series | v5.17 | https://lore.kernel.org/lkml/20211206135505.75045-1-kirill.shutemov@linux.intel.com/ | boot | 8260b9820f7050461b8969305bbd8cb5654f0c74..20f07a044a76aebaaa0603038857229b5c460d69 |
| TDX core support: TDX infrastructure​ ( eg: VE support, shared-mm) | v5.19 | https://lore.kernel.org/lkml/20220405232939.73860-1-kirill.shutemov@linux.intel.com/ | boot | 59bd54a84d15e9335de5b8abe7b3b9713a36b99b..b9c7ba58777acfd0892b808aea25074d46e0618f |
| TDX attestation | v6.2 | https://lore.kernel.org/all/20221116223820.819090-1-sathyanarayanan.kuppuswamy@linux.intel.com/ | attestation | 51acfe89af1118f906f9b68d95fdfb22832ac960..00e07cfbdf0b232f7553f0175f8f4e8d792f7e90 |
| More virtio hardening | v5.16 | https://lore.kernel.org/lkml/20211019070152.8236-1-jasowang@redhat.com/ | security | 6ae6ff6f6e7d2f304a12a53af8298e4f16ad633e..ef5c366fea30f64d52bb1c4c1e2959a5e6b66e88 |
| Packed virtqueue state support for vDPA | v5.14 | https://lore.kernel.org/lkml/20210602021536.39525-1-jasowang@redhat.com/ | security | 530a5678bc0083e84f99f38f77ced8fbb3d18434..efa08cb468cdd67855f63f341eac5f5f9ac93370 |
| Do not read from descriptor ring | v5.14 | https://lore.kernel.org/lkml/20210604055350.58753-1-jasowang@redhat.com/ | security | aeef9b4733c5c2356c75ba4f5c99e1a09ff1721d..72b5e8958738aaa453db5149e6ca3bcf416023b9 |
| Lazy accept | v6.5 | https://lore.kernel.org/lkml/20230606142637.5171-1-kirill.shutemov@linux.intel.com/ | performance | dcdfdd40fa82b6704d2841938e5c8ec3051eb0d6..75d090fd167acab4d7eda7e2b65729e877c0fd64 |
| #VE handler | v6.1 | https://lore.kernel.org/lkml/166734513448.7716.12910026848446212237.tip-bot2@tip-bot2/ | security | 373e715e31bf4e0f129befe87613a278fac228d3 |
| CCEL | v6.4 | https://lore.kernel.org/all/20230322191313.22804-1-sathyanarayanan.kuppuswamy@linux.intel.com/ | security | 4f855dcead6c5be0a48a2779eeecb170ec144534 |
| Mark TSC reliable | v6.6 | https://lore.kernel.org/all/169661218292.3135.7318812818696091080.tip-bot2@tip-bot2/T/ | security | 9ee4318c157b9802589b746cc340bae3142d984c |
| configfs-tsm: Attestation Report ABI | v6.7-rc1 | https://lore.kernel.org/all/169776458564.1705513.13069337506739791098.stgit@dwillia2-xfh.jf.intel.com/ | Attestation | db10cb9b574675402bfd8fe1a31aafdd45b002df..f4738f56d1dc62aaba69b33702a5ab098f1b8c63 |
| Fix soft lockups caused by parallel memory acceptance	| v6.6-rc7 | https://lore.kernel.org/all/20231016163122.12855-1-kirill.shutemov@linux.intel.com/ | Hotfix | 50e782a86c980d4f8292ef82ed8139282ca07a98 |

## Patches in review

| Patch description | patch version | Lore link | Category |
|-------------------|---------------|-----------|----------|
| Guest kdump and kexec support	| v5 | https://lore.kernel.org/lkml/20231222235209.32143-1-kirill.shutemov@linux.intel.com/ | Debug |
