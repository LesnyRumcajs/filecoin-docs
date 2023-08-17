---
description: >-
  The calibration network is the most realistic testnet simulation of the
  Filecoin mainnet.
---

# Calibration

The Calibration testnet is the most realistic simulation of the Filecoin mainnet.

Prospective storage providers can experience more realistic sealing performance and hardware requirements using final proofs constructions and parameters. Storage clients can store and retrieve _real data_ on the network. Clients can also participate in deal-making workflows and storage and retrieval functionality. The sector size on the Calibration testnet is the same as on the Filecoin mainnet; 32 GiB and 64 GiB sectors are supported. This testnet also includes the Filecoin EVM-runtime features found on the Filecoin mainnet.

**Large sector sizes**

A drawback of 32 GiB and 64 GiB sectors is that storage providers generally prefer deals that use a significant amount of the sector. This could cause issues for builders wanting to store less than 4 GiB of data.

[PiKNiK](https://www.piknik.com/) is running a Boost-enabled storage provider that will listen out for small deals to solve this issue. The PiKNiK SP will attempt to aggregate these deals into 32 GiB sectors. If a deal has yet to be bundled into a 32 GiB sector after 12 hours, then the PiKNiK SP will publish it in whatever state it is in.

Developers can reference pre-existing deals that are already available on the network. See the [`#fil-net-calibration-discuss` channel in the Filecoin Slack](https://filecoinproject.slack.com/archives/C01D42NNLMS) for support.

**Maintainer**: [Protocol Labs](https://protocol.ai)

## Genesis

* CAR File: `QmbHZuVjgtxvgtcE5H3FpE1ywEyawYmZcbx4Eh47WZ7YF8`
* Reset Timestamp: `1667326380` (`2022-11-01T18:13:00Z`)
* Genesis Block CID: `bafy2bzacecyaggy24wol5ruvs6qm73gjibs2l2iyhcqmvi7r7a4ph7zx3yqd4`
* SHA-1 Digest: `f9004d1266e0b023a018eb2fe6bb403cb8204df4`

## Network parameters

* Supported Sector Sizes: `32 GiB` and `64 GiB`
* Consensus Miner Min Power: `32 GiB`
* Epoch Duration Seconds: `30`
* Expected Leaders per Epoch: `5`
* WindowPoSt Proving Period: `2880`
* WindowPoSt Challenge Window: `60`
* WindowPoSt Period Deadlines: `48`
* Pre-Commit Challenge Delay: `150`

## Bootstrap peers

```plaintext
/dns4/bootstrap-0.calibration.fildev.network/tcp/1347/p2p/12D3KooWCi2w8U4DDB9xqrejb5KYHaQv2iA2AJJ6uzG3iQxNLBMy
/dns4/bootstrap-1.calibration.fildev.network/tcp/1347/p2p/12D3KooWDTayrBojBn9jWNNUih4nNQQBGJD7Zo3gQCKgBkUsS6dp
/dns4/bootstrap-2.calibration.fildev.network/tcp/1347/p2p/12D3KooWNRxTHUn8bf7jz1KEUPMc2dMgGfa4f8ZJTsquVSn3vHCG
/dns4/bootstrap-3.calibration.fildev.network/tcp/1347/p2p/12D3KooWFWUqE9jgXvcKHWieYs9nhyp6NF4ftwLGAHm4sCv73jjK
```

## Snapshots

* [Latest minimal snapshot](https://snapshots.calibrationnet.filops.net/minimal/latest.zst)

## Resources

* [Faucet](https://faucet.calibration.fildev.network/)
* [Stats Dashboard](https://stats.calibration.fildev.network/)
* [Slack Channel for Updates: #fil-network-announcements](https://filecoinproject.slack.com/archives/C01AC6999KQ)
* [Slack Channel for Questions: #fil-help](https://filecoinproject.slack.com/archives/CEGN061C5)
* [Latest lightweight snapshot](https://forest.chainsafe.io/calibnet/snapshot-latest) generated with [Forest](http://github.com/ChainSafe/forest) by [ChainSafe](https://chainsafe.io/)
