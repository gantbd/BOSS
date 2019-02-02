# BOSS

A repository to contain backups and patches for the xx-500 series of BOSS pedals.

files have a `.bel` extension, but appear to be standard JSON with the following schema:

    {
        "model": String,
        "version": String,
        "data: [
            "memo": String,
            "paramSet": [
                "UserBank%BankBNK": [ String ],  // 2 char hex strings, e.g. "6D"
                "UserBank%BankPAT(n)": [ String ],  // in field name n is 1-3, 475 2 char hex strings
            ],
            "patchNum": Integer
        ]
    }