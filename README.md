# sigstore-spacetime


- Verify `mgreau/cosign-test` container against a public key
```bash
$ cosign verify --key https://raw.githubusercontent.com/mgreau/sigstore-spacetime/main/cosign-test/cosign.pub docker.io/mgreau/cosign-test

Verification for index.docker.io/mgreau/cosign-test:latest --
The following checks were performed on each of these signatures:
  - The cosign claims were validated
  - The signatures were verified against the specified public key

[{"critical":{"identity":{"docker-reference":"index.docker.io/mgreau/cosign-test"},"image":{"docker-manifest-digest":"sha256:ba24d07c36df7e59d2368009e0ba01d2efaac65bf2c0eb8786ec31ea81a706c6"},"type":"cosign container image signature"},"optional":null}]
```