# ex2.0 • Solana Compute Marketplace

## Overview

Solana-based prototype of a decentralized compute marketplace built on the Solana network. Users can submit asks for compute, and providers can submit bids offering capacity. This creates a Solana based orders and runs a simple matching routine to pair compatible bids and asks. The project demonstrates how compute resources can be priced and exchanged directly on-chain.

## How It Works

Users create ask accounts describing the compute they need, the duration, and the maximum price they are willing to pay.
Providers create bid accounts describing the compute they can offer and the price they want.
When the matching instruction is called, the program checks existing orders and pairs any that satisfy each other’s requirements.
The frontend provides a basic interface for submitting orders and inspecting marketplace state.
This prototype focuses entirely on the marketplace logic; it does not execute real compute jobs.

## Project Structure
/ex2         Solana program written in Rust
/ex2front    Frontend built with React and TypeScript

## Running the Project
Solana Program
cd ex2
cargo build-sbf
solana program deploy target/deploy/ex2.so

## Frontend
cd ex2front
npm install
npm run dev


Before starting the frontend, update the configuration with the deployed program ID.
