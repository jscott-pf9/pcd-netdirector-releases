# PCD Network Director: appliance releases

**PCD Network Director** is a management plane for gateway appliances on Platform9 Private Cloud Director (PCD). Every tenant gets a hardened gateway VM with firewall, NAT, port forwarding and WireGuard VPN, managed from one web UI. Optional provider gateways add a shared BGP/ECMP tier for routable tenant networks.

This repository hosts the **appliance releases** used by the PCD App Catalog. Each release has three assets:

| Asset | What it is |
|---|---|
| `pcd-netdirector-<version>.qcow2` | The appliance image |
| `pcd-netdirector-<version>.qcow2.sha256` | Its SHA-256 checksum (`sha256sum` format) |
| `manifest.json` | The App Catalog manifest for that version |

## Install

In PCD, open **Extensions › Catalog** and choose **PCD Network Director**. The catalog imports the image from this repo, verifies its checksum, and deploys the appliance. Then open the web UI on port 8080 and finish first-run setup.

## Source

The source code is private. This repository contains only this README and release assets.
