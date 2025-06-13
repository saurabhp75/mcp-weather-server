<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

# MCP Weather Server

This is an MCP (Model Context Protocol) server project.

You can find more info and examples at https://modelcontextprotocol.io/llms-full.txt

## Project Structure

- `src/tools/` - Contains the weather tool implementation for fetching weather data
- `src/resources/` - Contains the weather resource implementation for providing cached weather data
- `src/prompts/` - Contains the weather report prompt implementation for generating weather reports
- `src/utils/` - Contains utility functions for interacting with weather APIs

## Dependencies

- @modelcontextprotocol/sdk - The official MCP SDK
- axios - HTTP client for making API requests
- dotenv - For environment variable management
- typescript - For TypeScript support
- ts-node - For running TypeScript directly
