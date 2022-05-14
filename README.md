# Solana NFT mint tools

See the full implementation in my blogs:

- [hackMD.io](https://hackmd.io/@happyeric77/ryrM1WpIc)
- [colorfulLife](https://colorfullife.ml/pages/diary/erics-daily-life/eric107/)

This project is inspired by SOLMEET workshop #3, please also refer to the instruction of SOLMEET resource

- [Youtube](https://www.youtube.com/watch?v=6SiQq-9J7lU)
- [Note](https://book.solmeet.dev/notes/complete-guide-to-mint-solana-nft)

Below is the original SOLMEET documentation:

# A Complete Guide to Mint Solana NFTs with Metaplex

- See this [doc](https://book.solmeet.dev/notes/complete-guide-to-mint-solana-nft) for more details

## Overview

- Generate profile pictures (pfp) from trait materials with configurable weights
- Use Metaplex Standard
- Upload pfp and metadata to Arweave, which is a decentralized storage network
- Mint NFT on [`solana-mf`](https://github.com/DappioWonderland/solana), a mainnet-fork developed by Dappio
- Some handy tools
  - `hashlips_art_generator`
  - `arweave-image-uploader`
  - `metaboss`

### Structure

```
├── 📂 solmeet-3-sandbox
│
├── 📂 hashlips_art_engine
│   │
│   ├── 📂 layers
│   │
│   └── 📂 build
│       │
│       ├── 📂 images
|       |
|       └── 📄 _metadata.csv
│
├── 📂 arweave-image-uploader
│   │
│   └── 📂 public
│       |
│       ├── 📂 images
│       |
│       ├── 📄 data.csv
│       |
│       └── 📄 arweave-uris.json
│
└── 📂 mint
    │
    ├── 📄 mint.js
    │
    └── 📄 mints.json
```
