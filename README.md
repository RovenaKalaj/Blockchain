# Module-18-Challenge
The provided code is a Python implementation of a blockchain ledger called PyChain. It is a simplified version of a blockchain and includes functionality to store and validate financial transaction records.

Here is a summary of the code:

The code defines a data class called Record that represents a financial transaction record. It has attributes such as sender (the sender's name), receiver (the receiver's name), and amount (the transaction amount).

The existing Block data class is modified to replace the data attribute with a record attribute of type Record. The Block class represents a block in the blockchain and includes attributes such as creator_id, prev_hash, timestamp, and nonce. The hash_block() method calculates the hash of the block using the record and other attributes.

The code also includes a PyChain class that represents the entire blockchain. It includes a list of Block objects as the chain and a difficulty attribute to control the proof-of-work mechanism.

The code uses the Streamlit library to create a user interface for interacting with the blockchain. The interface allows users to input the sender, receiver, and amount for each transaction record.

When the user clicks the "Add Block" button, a new Block object is created with a Record containing the user input. The block is then added to the blockchain using the proof-of-work mechanism.

The interface also provides options to view the blockchain and validate its integrity. The blockchain is displayed in a DataFrame format, showing the details of each block. The user can select a specific block to inspect its details.

Finally, the code includes instructions on how to run the Streamlit application, input transaction records, and test the blockchain validation process.

The code aims to demonstrate the basic functionality of a blockchain ledger, allowing users to store transaction records and validate the integrity of the blockchain.
