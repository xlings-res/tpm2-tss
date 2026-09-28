# tpm2-tss

xlings payload repacked from upstream binaries (conda-forge / Debian) by
[`.agents/tools/repack/repack.py`](https://github.com/openxlings/xim-pkgindex/tree/main/.agents/tools/repack).
Recipe: [`xim-pkgindex`](https://github.com/openxlings/xim-pkgindex) `pkgs/t/tpm2-tss.lua`.

Every release asset carries `PROVENANCE.md` (upstream artefacts, sha256, the exact command) and a `.sha256` sidecar.

## Sources

| artefact | sha256 | origin |
|---|---|---|
| https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-esys-3.0.2-0t64_4.1.3-1.2_amd64.deb | `87c0747c54e12be29c149145830385f5c6816b0fd962391858d63d70c921859e` | Debian libtss2-esys-3.0.2-0t64 4.1.3-1.2 amd64 |
| https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-mu-4.0.1-0t64_4.1.3-1.2_amd64.deb | `b7e1b9a05623f304aa82b4a577f8948e967f9212e5871c76bd88dd8e96b3e4ea` | Debian libtss2-mu-4.0.1-0t64 4.1.3-1.2 amd64 |
| https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-sys1t64_4.1.3-1.2_amd64.deb | `ffd806325106fb22cf479e65c6c74ef6c5db598a943dfd3b6a38b1edbdd55e99` | Debian libtss2-sys1t64 4.1.3-1.2 amd64 |
| https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-tcti-device0t64_4.1.3-1.2_amd64.deb | `e2c07f7258f52b611edb96945049dfc5dd0f066b9464cd2338716d73f78fc495` | Debian libtss2-tcti-device0t64 4.1.3-1.2 amd64 |

## Command

```
.agents/tools/repack/repack.py \
    --name tpm2-tss \
    --version 4.1.3 \
    --arch x86_64 \
    --src https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-esys-3.0.2-0t64_4.1.3-1.2_amd64.deb#87c0747c54e12be29c149145830385f5c6816b0fd962391858d63d70c921859e \
    --src https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-mu-4.0.1-0t64_4.1.3-1.2_amd64.deb#b7e1b9a05623f304aa82b4a577f8948e967f9212e5871c76bd88dd8e96b3e4ea \
    --src https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-sys1t64_4.1.3-1.2_amd64.deb#ffd806325106fb22cf479e65c6c74ef6c5db598a943dfd3b6a38b1edbdd55e99 \
    --src https://snapshot.debian.org/archive/debian/20241110T143611Z/pool/main/t/tpm2-tss/libtss2-tcti-device0t64_4.1.3-1.2_amd64.deb#e2c07f7258f52b611edb96945049dfc5dd0f066b9464cd2338716d73f78fc495 \
    --require lib/libtss2-esys.so.0 \
    --require lib/libtss2-mu.so.0 \
    --require lib/libtss2-sys.so.1 \
    --require lib/libtss2-tcti-device.so.0
```

