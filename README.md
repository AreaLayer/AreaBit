# AreaBit
Lending Bitcoin on RGB Network

# How works?

Scenario A

It defines a loan schema with borrower, lender, and amount fields, a loan contract with the defined schema, and loan metadata. It then generates a loan asset from the contract and metadata.

The borrower and lender addresses are generated using their public keys, and the borrower address is funded with 1 BTC.

Finally, the code generates three types of loan transitions: issuance, transfer, and redemption. The issuance transition issues the loan asset, the transfer transition transfers the asset from the borrower to the lender, and the redemption transition redeems the asset from the lender.

Scenario B

Discreet Log Contracts allow two parties to enter into a smart contract without revealing any sensitive information to each other.

To add DLCs to this code, you would need to modify the LoanSchema to include fields for the DLC parameters such as the oracle public key, the event descriptor, and the outcomes. You would also need to modify the LoanContract to include the DLC logic for the different stages of the loan contract such as the loan issuance, transfer, and redemption.

Once you have defined the DLC schema and contract, you can use the RGB library to generate the necessary DLC transactions and signatures. You would also need to integrate the oracle data source to retrieve the outcome of the event, which will determine the final payout to the parties involved.

Overall, adding DLCs to this code would make the loan contract more secure and privacy-preserving by eliminating the need for the parties to trust each other or a third-party escrow agent.

# Product

This product is in development

Based on RGB Protocol powered by LNP-BP Association
