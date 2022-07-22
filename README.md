## Installation
```
go install github.com/provenance-io/extkey/cmd/extkey@latest
```

# Encoding

## Key generation interactive
```
# Using interactive mode
 ▷▷ extkey encode --hrp tp --hd-path "m/44'/1'/0'/420'"
mnemonic: fly fly comfort
passphrase: 
seed: UeItRbah4gE-syrw1EaXVKyg3GKWqfZqOztWNAXfnUME-bMpjp4jT0YxzEBWBA33_QWDAmeFE1I_hNlt2xJJew==
hrp: tp
rootKey:
    address: tp148sw6szwkk3cj5fdudzyhamkj3juy0wx0pj2c0
    privateKey:
        base58: xprv9s21ZrQH143K2gAYPH8TS4wyWvQ4F99jm7cHbckUwKwvk75QpVx6VmqqZxgUno53xUWNbhnUy83RnPqSCa7hfKQFzmp1Lcsv2pp2PikLtHU
        bytes: 0488ADE40000000000000000003E02C49CF3397E45141E4C9BED309CE9630A2DC6C4C10892A8A71447C9AF79FE0088AAA01CC129E4C16BFE49AF8659B92CCA5D964F0A048BB1633F4514AB14850B4B6C702F
        bigInt: "61816016462973053634971943848394651064681471574639878248202317244753465607435"
    publicKey:
        base58: xpub661MyMwAqRbcFAF1VJfToCti4xEYebsb8LXtQ1A6VfUucuQZN3GM3aAKREjZt3ZFhQB2M5Le1FEfuhVQRQ8DgvmPkLjgKPMAFo5X923Ut1B
        bytes: 0488B21E0000000000000000003E02C49CF3397E45141E4C9BED309CE9630A2DC6C4C10892A8A71447C9AF79FE030F5D004B8355C738762E54CCD22ECBA7798A2327982BA412FDBFAC34F99B767354878D2E
        bigInt: "354325279253549169190772409736366026367206282379023929601832819184328435791475"
childKey:
    address: tp1ndh7g7xy48k52phkr3p37rnkazmc98zuv8fp38
    privateKey:
        base58: xprv9zqjpMDofQuSFaF8NsS2Ybq2Xndj9zB5PkKyS16JqWsvP8aQWELPkpBnTh6NUUFHmRqRxVpz3fT8S2ckHSRSQ8EDcS4ZifxwQsjWgJjn5GK
        bytes: 0488ADE40428508294800001A4F285FC31610476271F3EB344992EE7735D830235059FD301B1B5787A87A7B68F007531EE53DE80DCAA03BABDA2BA9FD00CC8CDDEAE481A61A996CC6E8EB417E1B327182390
        bigInt: "53008823667154757289335472780676933506146822681876901480085094723772554404275"
    publicKey:
        base58: xpub6Dq6DrkhVnTjU4KbUty2ujmm5pUDZStvkyFaEPVvPrQuFvuZ3meeJcWGJwjLjb666HDPxVg2SDTMuh6JVfP897z5VJxRoSf82koiPucLPDm
        bytes: 0488B21E0428508294800001A4F285FC31610476271F3EB344992EE7735D830235059FD301B1B5787A87A7B68F02416EF4140348D3BF8C0B2B81E1B1C75CF6E2B5335ECE3152106719A3728779095C9382A4
        bigInt: "261180551375323774831564216383503265774120811521638640313796615741160982804745"
```

## Key generation with env vars
```
# Using env vars
$ MNEMONIC="fly fly comfort" PASSPHRASE="" extkey encode --hrp tp --hd-path "m/44'/1'/0'/0'" 
seed: UeItRbah4gE-syrw1EaXVKyg3GKWqfZqOztWNAXfnUME-bMpjp4jT0YxzEBWBA33_QWDAmeFE1I_hNlt2xJJew==
hrp: tp
rootKey:
    address: tp148sw6szwkk3cj5fdudzyhamkj3juy0wx0pj2c0
    privateKey:
        base58: xprv9s21ZrQH143K2gAYPH8TS4wyWvQ4F99jm7cHbckUwKwvk75QpVx6VmqqZxgUno53xUWNbhnUy83RnPqSCa7hfKQFzmp1Lcsv2pp2PikLtHU
        bytes: 0488ADE40000000000000000003E02C49CF3397E45141E4C9BED309CE9630A2DC6C4C10892A8A71447C9AF79FE0088AAA01CC129E4C16BFE49AF8659B92CCA5D964F0A048BB1633F4514AB14850B4B6C702F
        bigInt: "61816016462973053634971943848394651064681471574639878248202317244753465607435"
    publicKey:
        base58: xpub661MyMwAqRbcFAF1VJfToCti4xEYebsb8LXtQ1A6VfUucuQZN3GM3aAKREjZt3ZFhQB2M5Le1FEfuhVQRQ8DgvmPkLjgKPMAFo5X923Ut1B
        bytes: 0488B21E0000000000000000003E02C49CF3397E45141E4C9BED309CE9630A2DC6C4C10892A8A71447C9AF79FE030F5D004B8355C738762E54CCD22ECBA7798A2327982BA412FDBFAC34F99B767354878D2E
        bigInt: "354325279253549169190772409736366026367206282379023929601832819184328435791475"
childKey:
    address: tp1wjccte6zcr0d9d8l5mjj5ju6rmlcywlt02tlpn
    privateKey:
        base58: xprv9zqjpMDofQu7oDsEZEoP8sFrrvqewMi4s8ntBLthjaGfnwe8sCXdjgqYH5HQZXDeHbtsS3mdqdkaFAGVNJ6Xde48hkUsfbtUsJTQKyvBVJv
        bytes: 0488ADE4042850829480000000FEB0AB4988EAE6538E60190EBF17678B0F2E590ED1D88D5D7CD8E50B63AC23EF00436F8E356F0E13B8007D668625ED6B61FC65B8286778452DE55F124DD934CB9FCCE76EDF
        bigInt: "30502062367823121628620232764791700029549832820376726752590340403318586919839"
    publicKey:
        base58: xpub6Dq6DrkhVnTR1hwhfGLPW1CbQxg9LpRvEMiUyjJKHuoefjyHQjqtHVA28NCY3YqM35fd1LyG5jkAaYZbHciHhDdJPxSux97o1nvBgvcww7o
        bytes: 0488B21E042850829480000000FEB0AB4988EAE6538E60190EBF17678B0F2E590ED1D88D5D7CD8E50B63AC23EF033BC1E08A7DAF3D04F704B43DD53FF9E4C4FDC9855B416881859B3808EFEDD34543BDE2A2
        bigInt: "374405276986753977850763764723578643711636570020048640824572441823815521915717"
```

# Decoding

## Decoding xprv keys
```
$ extkey decode --hrp tp xprv9zqjpMDofQuSFaF8NsS2Ybq2Xndj9zB5PkKyS16JqWsvP8aQWELPkpBnTh6NUUFHmRqRxVpz3fT8S2ckHSRSQ8EDcS4ZifxwQsjWgJjn5GK
address: tp1ndh7g7xy48k52phkr3p37rnkazmc98zuv8fp38
xkey:
    private: xprv9zqjpMDofQuSFaF8NsS2Ybq2Xndj9zB5PkKyS16JqWsvP8aQWELPkpBnTh6NUUFHmRqRxVpz3fT8S2ckHSRSQ8EDcS4ZifxwQsjWgJjn5GK
    public: xpub6Dq6DrkhVnTjU4KbUty2ujmm5pUDZStvkyFaEPVvPrQuFvuZ3meeJcWGJwjLjb666HDPxVg2SDTMuh6JVfP897z5VJxRoSf82koiPucLPDm
    depth: 4
    depthLoc: m/44/coin/account/*change/index
    chaincode: F285FC31610476271F3EB344992EE7735D830235059FD301B1B5787A87A7B68F
    fingerprint: "28508294"
```

## Decoding xpub keys
```
$ extkey decode --hrp tp xpub6Dq6DrkhVnTjU4KbUty2ujmm5pUDZStvkyFaEPVvPrQuFvuZ3meeJcWGJwjLjb666HDPxVg2SDTMuh6JVfP897z5VJxRoSf82koiPucLPDm
address: tp1ndh7g7xy48k52phkr3p37rnkazmc98zuv8fp38
xkey:
    public: xpub6Dq6DrkhVnTjU4KbUty2ujmm5pUDZStvkyFaEPVvPrQuFvuZ3meeJcWGJwjLjb666HDPxVg2SDTMuh6JVfP897z5VJxRoSf82koiPucLPDm
    depth: 4
    depthLoc: m/44/coin/account/*change/index
    chaincode: F285FC31610476271F3EB344992EE7735D830235059FD301B1B5787A87A7B68F
    fingerprint: "28508294"
```
