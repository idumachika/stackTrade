 A peer-to-peer digital asset exchange smart contract built on the Stacks blockchain using Clarity.This contract allows users to list, buy, trade, and manage digital content securely with decentralized ownership.

📌 Features

✅ List Digital Content - Users can register digital assets with pricing and metadata.✅ Trade Assets - Peer-to-peer buying and selling of digital content.✅ Access Management - Buyers receive secure access tokens for purchased content.✅ Fee Mechanism - Transaction fees are deducted from purchases.✅ Modify Listings - Owners can update pricing or remove assets from the marketplace.✅ Trader Reputation Tracking - Records trade history and reputation scores.

🚀 Getting Started

1️⃣ Prerequisites

Ensure you have the following installed:

Node.js (for testing)

Clarinet (for running Clarity contracts)

Vitest (for testing)

2️⃣ Clone the Repository

git clone https://github.com/your-username/digital-asset-exchange.git
cd digital-asset-exchange

3️⃣ Install Dependencies

npm install

4️⃣ Run the Smart Contract Locally

clarinet test

🛠️ Contract Functions

📌 Public Functions

Function

Description

register-content(asking-price, summary, content-type, access-token)

Lists a new digital asset for sale.

acquire-content(item-id)

Purchases a digital asset.

retrieve-access-token(item-id)

Retrieves access credentials for purchased content.

modify-price(item-id, updated-price)

Updates the price of a listed item (owner only).

delist-content(item-id)

Removes an asset from the marketplace.

adjust-fee-rate(new-rate)

Admin function to change the exchange fee.

📌 Read-Only Functions

Function

Description

get-content-info(item-id)

Retrieves details about a listed asset.

get-trader-info(participant)

Fetches trade history and reputation of a trader.

get-exchange-stats()

Returns the total number of completed trades.

get-current-fee()

Gets the current transaction fee rate.

🧪 Running Tests

We use Vitest for unit testing.

1️⃣ Run Tests

npx vitest

2️⃣ Example Test Cases

✅ Registering Digital Content

✅ Acquiring an Asset

✅ Retrieving Access Token

✅ Preventing Unauthorized Modifications

✅ Adjusting Exchange Fees (Admin Only)