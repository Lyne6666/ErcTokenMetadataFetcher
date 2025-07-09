# ErcTokenMetadataFetcher

## Description

A curated collection of NFT smart contracts utilizing Cairo for provable ownership and secure transactions on StarkNet, leveraging its STARK-based validity proofs for enhanced scalability and data integrity.

## Features

- Fetches ERC-721 and ERC-1155 token metadata using Ethers.js or Web3.js libraries.
- Caches fetched metadata in a Redis database to minimize API calls and improve response times.
- Implements a rate limiting mechanism using the Token Bucket algorithm to prevent exceeding API rate limits.
- Supports configurable retry strategies with exponential backoff for handling temporary API errors.
- Validates metadata JSON schema against a pre-defined schema to ensure data integrity.
- Provides a GraphQL API endpoint for querying token metadata based on contract address and token ID.
- Integrates with IPFS gateways to retrieve metadata stored on the InterPlanetary File System.
- Employs asynchronous task queues (e.g., Celery) to handle metadata fetching in the background.
## Installation

```bash
pip install git+https://github.com/Lyne6666/ErcTokenMetadataFetcher.git
```

## Usage

```bash
python -m erctokenmetadatafetcher --verbose
```

## Contributing

We welcome contributions! Here's how to get started:

1. Fork this repository
2. Create a new branch for your feature (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some awesome feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.
