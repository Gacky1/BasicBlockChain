# BasicBlockChain
 My first ever basic blockchain trial project.
1. What is a blockchain?
   A blockchain is like a digital ledger or record book. Imagine a chain of blocks, where each block contains some information. Once a block is added to the chain, its information can't be changed without changing all the blocks that come after it. This makes blockchains very secure and tamper-resistant.

2. What does our project do?
   Our project creates a very simple version of a blockchain. It's a webpage where you can:
   - Enter some information (we call this "data")
   - Add this information as a new "block" to our chain
   - See all the blocks in our chain displayed on the page

3. Key parts of our project:

   a. Blocks:
      - Each block is like a container that holds some information.
      - In our project, a block contains:
        * An index (its position in the chain)
        * A timestamp (when it was created)
        * Some data (the information you enter)
        * A "hash" (like a unique fingerprint for the block)
        * The "hash" of the previous block (this is how blocks are linked)

   b. The Chain:
      - Our blockchain starts with a special first block called the "Genesis block".
      - Every time you add information, a new block is created and added to the end of the chain.
      - Each new block contains a reference to the block before it (the "previous hash"). This creates the "chain" in blockchain.

   c. Hashing:
      - A hash is like a digital fingerprint for data.
      - In our project, we create a hash for each block based on its content.
      - If anything in the block changes, its hash will change too.
      - This helps ensure the integrity of our blockchain - if someone tries to change a past block, it will be obvious because all the subsequent hashes would change.

4. How to use the project:
   - When you open the webpage, you'll see an input box and an "Add Block" button.
   - Type some information into the input box.
   - Click "Add Block". This will:
     * Create a new block with your information
     * Add this block to the end of the chain
     * Show you the updated blockchain on the page

5. What you'll see:
   - Below the input area, you'll see a display of all the blocks in the chain.
   - For each block, you'll see its index, when it was created, the data it contains, its own hash, and the hash of the block before it.

This project is a very simplified version of a blockchain. Real blockchains used for cryptocurrencies or other applications are much more complex. They involve many computers working together, complex algorithms for adding blocks, and mechanisms to ensure everyone agrees on the state of the blockchain.

The main idea to take away is that a blockchain is a way of storing information that makes it very difficult to change past records without detection. This property makes blockchains useful for many applications beyond just cryptocurrencies, like supply chain management, voting systems, and more.