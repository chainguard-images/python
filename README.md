# python

<!---
Note: Do NOT edit directly, this file was generated using https://github.com/chainguard-images/readme-generator
-->

[![CI status](https://github.com/chainguard-images/python/actions/workflows/release.yaml/badge.svg)](https://github.com/chainguard-images/python/actions/workflows/release.yaml)

This is a minimal Python image based on Alpine, using Python apks available on the Alpine Community repositories (not built from source as of now).<br/><br/>While this image is being developed, we will stick to the latest stable Python version which at this moment is `3.10.7`. Supported versions in the long term are TBD.

## Get It!

The image is available on `cgr.dev`:

```
docker pull cgr.dev/chainguard/python:latest
```

## Supported tags

| Tag | Digest | Arch |
| --- | ------ | ---- |
| `migration` `migration-20221126` | `sha256:2267da75e3fe01d6f215fc51fcbf268c2105da1eb9739f83ef4dbc774bd51259`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:2267da75e3fe01d6f215fc51fcbf268c2105da1eb9739f83ef4dbc774bd51259) | `amd64` |
| `migration-20221119` | `sha256:bd5fb01c0e49167e21f2a4be26a1e58262b391813bed99bb7fd81a1ec2457974`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:bd5fb01c0e49167e21f2a4be26a1e58262b391813bed99bb7fd81a1ec2457974) | `amd64` |
| `migration-20221121` | `sha256:0ccde133cd574742173984fbdc4768d728bcd45d6f0685fc2b961b1647cc27c1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:0ccde133cd574742173984fbdc4768d728bcd45d6f0685fc2b961b1647cc27c1) | `amd64` |
| `migration-20221123` | `sha256:320632b276a7e69039cd9f97bc7172c82a6e9228cf5bb84d5e718a14404f7613`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:320632b276a7e69039cd9f97bc7172c82a6e9228cf5bb84d5e718a14404f7613) | `amd64` |
| `migration-20221125` | `sha256:ca1dede10d2b15036ae0ea9f5459419df5a2de171068d1ec2230f8a03f9a8d41`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:ca1dede10d2b15036ae0ea9f5459419df5a2de171068d1ec2230f8a03f9a8d41) | `amd64` |
| `latest` | `sha256:beaa45720634ff3d21e68f850225b7943c1882a3463388cfca9c6a5e7fb1353c`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:beaa45720634ff3d21e68f850225b7943c1882a3463388cfca9c6a5e7fb1353c) | `386` `amd64` `arm64` `armv6` `armv7` `ppc64le` `riscv64` `s390x` |
| `migration-20221118` | `sha256:0012ef5bfc2d6791c962b1cc99cc2c2934cf216ca5937c9eb2a80935c8ad898a`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:0012ef5bfc2d6791c962b1cc99cc2c2934cf216ca5937c9eb2a80935c8ad898a) | `amd64` |
| `migration-20221120` | `sha256:c43a298d7a5442d3a94b2c09a5eb1690e0bc0d82f7bc967409de0e42668541ef`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:c43a298d7a5442d3a94b2c09a5eb1690e0bc0d82f7bc967409de0e42668541ef) | `amd64` |
| `migration-20221122` | `sha256:2fb92368254ec422ead3d189999868e1c35daf729178681766c4e827dfd6fdf4`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:2fb92368254ec422ead3d189999868e1c35daf729178681766c4e827dfd6fdf4) | `amd64` |
| `migration-20221124` | `sha256:335f4780b3e6b2137db65a0da5df15ab8491af3f2e05c7af00d6f4a212d402b7`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:335f4780b3e6b2137db65a0da5df15ab8491af3f2e05c7af00d6f4a212d402b7) | `amd64` |


## Usage

To try out the image, run:

```shell
docker run --rm cgr.dev/chainguard/python python -VV
```

Python version installed 
```
Python 3.10.7 (main, Sep 11 2022, 22:42:41) [GCC 12.1.1 20220630]
```

Pip Version installed 

```shell 
docker run --rm cgr.dev/chainguard/python pip -V
```

```shell
pip 22.2.2 from /usr/lib/python3.10/site-packages/pip (python 3.10)
```


## Signing

All Chainguard Images are signed using [Sigstore](https://sigstore.dev)!

<details>
<br/>
To verify the image, download <a href="https://github.com/sigstore/cosign">cosign</a> and run:

```
COSIGN_EXPERIMENTAL=1 cosign verify cgr.dev/chainguard/python:latest | jq
```

Output:
```
Verification for cgr.dev/chainguard/python:latest --
The following checks were performed on each of these signatures:
  - The cosign claims were validated
  - Existence of the claims in the transparency log was verified offline
  - Any certificates were verified against the Fulcio roots.
[
  {
    "critical": {
      "identity": {
        "docker-reference": "ghcr.io/chainguard-images/python"
      },
      "image": {
        "docker-manifest-digest": "sha256:beaa45720634ff3d21e68f850225b7943c1882a3463388cfca9c6a5e7fb1353c"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "3fcfd15aea19b77367241514c539db4a8a9499cb",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/python",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQCEHw/A/JVV3R4YRhuUsRxui83kvNRPJmV4Jhe0S9eclQIgK62eEK3u5hcoRFgi8yHZE8EmQA7HHXyKRn504fcOhDo=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJmMGE2NTFiYmIyZjJmODY4MWIwZjQyYzA2M2U2YjZhMTlkNWI0YjhjMGJlZTc2MTY0ZTUxYWYxM2YxNmIwODgzIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUURPeEhQenNNNVlOdm04TGFpR09OQXF1ZjhSTWE4OHc1Y2QwVUticllUUEd3SWdSbm9acytYakEyUFZIRzZrM2U4cE1iVzZQV05qczBEV1l6K2xLZ01icXRVPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnlSRU5EUVhwSFowRjNTVUpCWjBsVlZFdGlVa0UzTkZNd0wycElWM0ZNUjJ0amJtRldhRUZNVUV4RmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RKTlJFRjRUMVJKZVZkb1kwNU5ha2w0VFZSSk1rMUVRWGxQVkVsNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZCV0hkTVpHWlRTbGxSZVZFdmRGSlRhRmt6Y0VSMlJXVm9VR2xqZW1reVVsaEZLMDBLWmxJeFNUTjBjM3AwTWs1S1JXTk1VbnBEVjNJMFdrTkZSbmMwSzJkMFdpOXZSV0Z0YVZsdFlYSm5WRUZJZWs5SVMyRlBRMEZzUVhkblowcE5UVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZUZWtsSENrTkhRVlpyTkc5alkwTklTbUZ1WlVsU2NGb3JUbGs0ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJGQldVUldVakJTUVZGSUwwSkdOSGRZU1ZwaFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6UWpWa1IyaDJZbWs0ZFZveWJEQmhTRlpwVEROa2RtTnRkRzFpUnprelkzazVlVnBYZUd4WldFNXNURzVzYUdKWGVFRmpiVlp0Q21ONU9XOWFWMFpyWTNrNWRGbFhiSFZOUkd0SFEybHpSMEZSVVVKbk56aDNRVkZGUlVzeWFEQmtTRUo2VDJrNGRtUkhPWEphVnpSMVdWZE9NR0ZYT1hVS1kzazFibUZZVW05a1Ywb3hZekpXZVZreU9YVmtSMVoxWkVNMWFtSXlNSGRHWjFsTFMzZFpRa0pCUjBSMmVrRkNRV2RSU1dNeVRtOWFWMUl4WWtkVmR3cE9aMWxMUzNkWlFrSkJSMFIyZWtGQ1FYZFJiMDB5V21wYWJWRjRUbGRHYkZsVVJUVlphbU16VFhwWk0wMXFVWGhPVkVVd1dYcFZlazlYVW1sT1IwVTBDbGxVYXpCUFZHeHFXV3BCWTBKbmIzSkNaMFZGUVZsUEwwMUJSVVZDUVRWRVkyMVdhR1JIVldkVmJWWnpXbGRHZWxwVVFXMUNaMjl5UW1kRlJVRlpUeThLVFVGRlJrSkNhR3BoUjBad1ltMWtNVmxZU210TVYyeDBXVmRrYkdONU9YZGxXRkp2WWpJMGQwaFJXVXRMZDFsQ1FrRkhSSFo2UVVKQ1oxRlFZMjFXYlFwamVUbHZXbGRHYTJONU9YUlpWMngxVFVsSFMwSm5iM0pDWjBWRlFXUmFOVUZuVVVOQ1NIZEZaV2RDTkVGSVdVRXpWREIzWVhOaVNFVlVTbXBIVWpSakNtMVhZek5CY1VwTFdISnFaVkJMTXk5b05IQjVaME00Y0Rkdk5FRkJRVWRGYzFVeVZEUkJRVUZDUVUxQlVucENSa0ZwUVhaUFMycE1UalF3YlhSNmJFMEtTMnRRVjFnNVZuTmxaWGhhTWxCa2ExSTFaRGQzYVZJeVUxcHpjV0pSU1doQlNrOU5jRXhqSzJOUk9ITmpOamhXUm5aUlprdEJkelpOU25kRWNYVTFad3BhYkVWcGFFWnlZamwxTjBOTlFXOUhRME54UjFOTk5EbENRVTFFUVRKclFVMUhXVU5OVVVSRlFsaHViR012WmtOVWFXUldWa1pPTW5OWFRsRkNTemt3Q2psTFNUbEpjVkZ0WW5CcE5rWk9TRmQ2VTBwVlpteDZSMVJoY2prM2RFbENTVU56ZDFOTE9FTk5VVU52TDJJck1reHFkVzQzTWpJNGJGUmlXQ3RGUkRjS2FDdFFaMlJVVkhodlJFTkZVRXhGTDFoV0syOHdaMWRPUWxoSVptZzRUa3cwWWt3eGJFMUdUMHB0TkQwS0xTMHRMUzFGVGtRZ1EwVlNWRWxHU1VOQlZFVXRMUzB0TFFvPSJ9fX19",
          "integratedTime": 1669421994,
          "logIndex": 7857221,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/python/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/python",
      "githubWorkflowSha": "3fcfd15aea19b77367241514c539db4a8a9499cb",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3551408833",
      "sha": "3fcfd15aea19b77367241514c539db4a8a9499cb"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

