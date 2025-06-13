# MCP Weather Server

An MCP (Model Context Protocol) server that provides weather information through tools, resources, and prompts using the official MCP TypeScript SDK.

## Features

- **Weather Tool**: Fetches current weather data for any location
- **Weather Resource**: Provides standardized weather data with caching
- **Weather Report Prompt**: Generates custom weather reports

## Getting Started

### Prerequisites

- Node.js (v16 or later)
- npm or yarn
- A Weather API key (from [WeatherAPI.com](https://www.weatherapi.com))

### Installation

1. Clone this repository
2. Install dependencies:
   ```
   npm install
   ```
3. Copy the environment example file and fill in your API key:
   ```
   cp .env.example .env
   ```
   Edit the `.env` file to add your Weather API key.

### Running the Server

Development mode:

```
npm run dev
```

Production mode:

```
npm run build
npm start
```

## API Usage

### Weather Tool

The `get_weather` tool can be called to get weather information for a specific location:

```json
{
  "name": "get_weather",
  "parameters": {
    "location": "New York"
  }
}
```

### Weather Resource

The weather resource can be accessed with:

```json
{
  "name": "weather_data",
  "parameters": {
    "location": "London"
  }
}
```

### Weather Report Prompt

The weather report prompt can be customized:

```json
{
  "name": "weather_report",
  "parameters": {
    "location": "Tokyo",
    "detailLevel": "detailed",
    "format": "factual"
  }
}
```
