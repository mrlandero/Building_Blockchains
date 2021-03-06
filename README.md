# Building_Blockchains
Will use Python and Streamlit to create an application that lets users add blocks to the blockchain and then validates the entire blockchain.

---

## Technologies

This project leverages python 3.7 with the following packages:

**[Streamlit Library](https://docs.streamlit.io/)** - Streamlit is an open-source Python library that makes it easy to create and share beautiful, custom web apps for machine learning and data science.<br>

**[Dataclasses Library](https://docs.python.org/3/library/dataclasses.html)** - This module provides a decorator and functions for automatically adding generated special methods such as __init__() and __repr__() to user-defined classes.<br>

**[Typing Library](https://docs.python.org/3/library/typing.html)** - This module provides runtime support for type hints. The most fundamental support consists of the types Any, Union, Callable, TypeVar, and Generic.<br>

**[Datetime Library](https://docs.python.org/3/library/datetime.html)** - The datetime module supplies classes for manipulating dates and times.<br>

**[Pandas Library](https://pandas.pydata.org/)** - pandas is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool,
built on top of the Python programming language.<br>

**[Hashlib Library](https://docs.python.org/3/library/hashlib.html)** - This module implements a common interface to many different secure hash and message digest algorithms. Included are the FIPS secure hash algorithms SHA1, SHA224, SHA256, SHA384, and SHA512.<br>

## Installation Guide

Before running the application first install the following dependencies:

First, we need to verify that we have Streamlit installed. From your terminal, type the following command:

```python
conda list streamlit
```

If it is installed on your computer, you should see a similar message to this:

![Streamlit List](images/streamlit_list.png)

If it is not installed on your computer, you need to install it with the following command:

```python
pip install streamlit
```

That takes care of Streamlit.

Now, let's verify that the Typing Library is installed. From your terminal, type the following command:

```python
conda list typing
```
If it is installed on your computer, you should see a similar message to this:

![Typing List](images/typing_list.png)

If it is not installed on your computer, you need to install it with the following command:

```python
pip install typing
```

We are done installing the Typing Library

Next, let's verify that the Pandas Library is installed. From your terminal, type the following command:

```python
conda list pandas
```
If it is installed on your computer, you should see a similar message to this:

![Pandas List](images/pandas_list.png)

If it is not installed on your computer, you need to install it with the following command:

```python
pip install pandas
```

We are done with the Pandas installation.

We are now ready to start using the application.

---

## Usage

To use the 'Building_Blockchains' application, simply clone the repository and type **streamlit run pychain.py** in your terminal.

Step 1: Select the block difficulty from the sidebar. This will increase the difficulty of the calculation that must be complete before adding the next block.

![Block Difficulty](images/block_difficulty.png)

Step 2: Fill in the `sender` area with the numerical ID of the person sending information.

![Sender ID](images/sender_id.png)

Step 3: Fill in the `receiver` area with the numerical ID of the person receiving information.

![Receiver ID](images/receiver_id.png)

Step 4: Fill in the `amount` area with the value of the transaction.

![Amount](images/amount.png)

Step 5: Click the `Add Block` button to add the new block to the end of the chain.

![Add Block](images/add_block.png)

Step 6: Review the PyChain Ledger to verify the new block was added to the chain.

![PyChain DF](images/pychain_df.png)

As we can see in the preceding image, the `Sender ID` is 50. The `Receiver ID` is 854.The `amount` sent was $525.00. 
Once we click the `Add Block` button, we should see our new block attached to the end of the table. We can see that clearly in this example. The "0" block is the Genesis block, or the first block of the chain. However, the "1" block in the table displays the information of our newly attached block. 

Congratulations! You just added your first block to the blockchain. 

Step 7: Use the `Block Inspector` section to have another way to verify the creation of the new block. 

![Block Inspector](images/block_inspector.png)

For this example, we see that we clicked on the record for the newly created block. It has the same information as the PyChain Ledger from the previous step, however it also provides 2 additional pieces of information: 1) Displays the `prev_hash` from the preceding block. 2) Displays the `nonce` that solved the math calculations, given the difficulty level. 

Step 8: Click on `Validate Chain` to verify that the entire chain is valid and secure. 

![Validate Chain](images/validate_chain.png)

In this example we can see that the result from clicking the `Validate Chain` button is `True`. This means that our blockchain has been validated and all of the information is verified. This means that the blockchain is secure for the time being. 
If the result had been `False`, this is a redflag that something in one of the block might have changed, making the blockchain not secure. 

Once you complete all of these steps, repeat them in order to add a new block, and for every block thereafter. 

You can now add blocks to our PyChain and you can validate the information in the chain to verify its security. 

---

## Contributors

**Created by:** Tony Landero<br>
**Email:** mr.landero@gmail.com<br>

---

## License

MIT