Project Description: Building a Custom ERC-20-Like Token Contract
In this guided project, i implemented a simple Solidity smart contract that mimics the basic functionality of an ERC-20 token. The contract demonstrates how to manage balances, mint tokens, and transfer tokens securely on the Ethereum blockchain. Here’s an overview of the contract's features and learning outcomes:

Project Features
Mapping for Balances:

A mapping is used to store the token balances for each Ethereum address, associating addresses with their respective token amounts.
Example: balances[address] retrieves the balance of a specific address.
Total Token Supply:

A uint256 variable totalSupply tracks the total number of tokens minted in the contract.
This is public, allowing anyone to query the total token supply.
Owner Control:

The contract implements permission control by assigning the deployer of the contract (msg.sender) as the owner in the constructor.
Only the owner can mint new tokens, ensuring centralized control over token creation.
Token Minting:

The mint function allows the owner to issue new tokens to a specified address.
It updates both the recipient’s balance and the totalSupply.
Balance Query:

The balanceOf function provides a public interface to check the balance of any address in the contract.
Token Transfers:

The transfer function allows users to send tokens to other addresses.
It ensures the sender has enough balance before completing the transfer.
