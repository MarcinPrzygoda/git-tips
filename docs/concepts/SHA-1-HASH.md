# 📋 SHA-1 HASH

Git generates a **checksum** for each changeset.

Checksum algorithms **convert data** into a **simple number** (checksum).

Same data **always return** the same checksum. It's used to guarantee **data integrity**.

Changing data would **change checksum**. You also can't change **metadata** such as: commit message, commit author or parent of the commit without also changing checksum.

Git uses **SHA-1 hash algorithm** to create checksums which is **40-character hexadecimal string** (0-9, a-f) for example: `7da15ff2f381d33118ac450bf35b9cf8f4fa2830`.