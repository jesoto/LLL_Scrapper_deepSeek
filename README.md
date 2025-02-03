# Web Scraping with LLM-Powered Extraction

This repository contains a Python script that extracts structured data from the **LM Arena Leaderboard** using **crawl4ai** and an LLM-based extraction strategy.

## Features
- Uses `crawl4ai` for web crawling and `deepseek/deepseek-chat` for data extraction.
- Extracts structured data from the leaderboard table.
- Bypasses caching and processes content efficiently.
- Outputs extracted data in JSON format.

## Installation

Make sure you have Python 3.8+ installed, then install dependencies:

```sh
pip install crawl4ai pydantic asyncio
```

## Configuration

Set your **DeepSeek API Token** as an environment variable:

```sh
export DEEPSEEK_API="your_api_key_here"
```

## Usage

Run the script using:

```sh
python main.py
```

## Output Example

If successful, the script will output extracted items in JSON format:

```json
{
    "rank": 1,
    "model": "Example Model",
    "arena score": 98.5,
    "95% CI": "97.5 - 99.5",
    "Votes": 1500,
    "Organization": "Example Org",
    "License": "MIT"
}
```

## File Structure

```
.
├── main.py  # Main script
├── README.md  # Documentation
└── requirements.txt  # Dependencies
```

## Dependencies
- `crawl4ai`
- `pydantic`
- `asyncio`

## License
This project is licensed under the MIT License.

