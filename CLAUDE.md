# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Cross-Site WebSocket Hijacking (CSWH) vulnerability testing tool. It consists of a single HTML file (`CSWH-test.html`) that provides a web-based interface for security professionals to test WebSocket applications for CSWH vulnerabilities.

## Architecture

- **Single-file application**: The entire tool is contained in `CSWH-test.html`
- **Client-side only**: Pure HTML/CSS/JavaScript with no backend dependencies
- **Cyberpunk-themed UI**: Dark mode interface with neon green/cyan color scheme using "Press Start 2P" and "Roboto Mono" fonts
- **Real-time WebSocket testing**: Establishes connections to target WebSocket servers and logs all activity

## Key Components

- **Connection Setup**: Form to input WebSocket URLs and establish connections
- **Traffic Injection**: Interface to send custom messages to connected WebSocket servers
- **Activity Log**: Real-time display of connection events, sent/received messages with copy-to-input functionality
- **JSON Formatting**: Built-in JSON formatter for structured data testing

## Development Notes

- No build process required - static HTML file can be opened directly in browsers
- No package.json or dependencies - uses external CDN fonts only
- Security testing tool - designed for defensive security analysis only
- Educational purpose - includes comprehensive documentation about CSWH vulnerabilities

## Usage

Open `CSWH-test.html` directly in a web browser. The tool is ready to use without any setup or installation.