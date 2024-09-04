![Periscope Logo](./periscope.png)

# Periscope

## Dive Deep into Liquidity Pool Data

Periscope is a powerful Solana blockchain data pipeline designed to provide deep insights into DeFi liquidity pool data. Built with Rust, Apache Arrow, and DataFusion, Periscope offers a modular and extensible framework for collecting, processing, and analyzing data from various liquidity pools.

### Features

- **Modular Architecture**: Easily extendable to support multiple DeFi protocols (Orca, Raydium, Meteora, and more).
- **Surface Scan**: Get quick, high-level metrics across all supported liquidity pools.
- **Deep Dive Analysis**: Perform in-depth analysis on specific pools or across the entire DeFi landscape.
- **Efficient Data Processing**: Utilizes Apache Arrow and DataFusion for high-performance data operations.
- **Parquet Output**: Store processed data in the efficient Parquet file format for further analysis or long-term storage.

### Getting Started

#### Prerequisites

- Rust (latest stable version)
- Solana CLI tools

#### Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/periscope.git
   cd periscope
   ```

2. Build the project:

   ```sh
   cargo build --release
   ```

3. Run Periscope:
   ```sh
   cargo run --release
   ```

### Usage

Periscope provides a command-line interface for interacting with the data pipeline. Here are some example commands:

- Perform a surface scan across all supported pools:

  ```sh
  periscope surface-scan
  ```

- Run a deep analysis on a specific pool:

  ```sh
  periscope analyze --pool orca
  ```

- Export data to Parquet format:
  ```sh
  periscope export --format parquet --output ./data
  ```

### Configuration

Periscope can be configured via a `config.toml` file in the project root. Here you can specify RPC endpoints, pool addresses, and other settings.

### Contributing

We welcome contributions to Periscope! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) file for details on how to get started.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Acknowledgments

- The Solana Foundation for their excellent blockchain infrastructure
- The Apache Arrow and DataFusion teams for their powerful data processing tools

---

Built with ❤️ by Fodé Diop
