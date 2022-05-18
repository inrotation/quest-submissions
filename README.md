0xa63f66bee1fea68f

# Chapter 1, Day 1:
1. A Blockchain is an open, decentralized, public database which stores data into linked chunks (or, blocks) as opposed to your usual database which stores them in tables. The most common type of data stored on blockchains are ledgers for transactions, however other types may be used.
2. Smart Contracts are transaction protocols on the blockchain which execute terms of a contract. They are speedy,  extremely secure, and - for better or worse - irreversible once deployed.
3. Transactions are used to change blockchain data while Scripts are used merely to view blockchain data. 


# Chapter 1, Day 2:
The Pillars of Cadence programming language (& their usefulness!)

1. Safety and Security - self-explanatory; should be the hallmark of any smart contract language worth its muster!  
2. Clarity - code that is simple for developers to express intent and readers to comprehend serve to ensure safety 
3. Approachability - Similarities in syntax to other programming languages ensures a low barrier to entry for interested software developers.	
4. Developer Experience - clarity in error messages will help developers debug sans frustration. 
5. Resource Oriented Programming

# Chapter 2, Day 1:

## Quest 1:

<img width="627" alt="Quest 1" src="https://user-images.githubusercontent.com/26890946/166808408-1db102cd-32e7-41db-a63f-0dcc588d8d85.png">

## Quest 2:

<img width="877" alt="Quest 2" src="https://user-images.githubusercontent.com/26890946/166808450-e5328858-0b0d-4121-87de-ae08473aead2.png">


# Chapter 2, Day 2:

## Quests

1. We wouldn’t call _changeGreeting_ in a script because scripts are meant to view data, and _changeGreeting_ is meant to modify data (more specifically, here: our _greeting_ variable)
2. In the _prepare_ phase of the transaction **AuthAccount** is meant to access the data in one’s account. 
3. In the _Prepare_ phase of a transaction, we are accessing data in someone’s account, while in the _Execute_ phase we are changing some data
4.
![1](https://user-images.githubusercontent.com/26890946/167965356-4757d2d3-ec9a-4b3a-adc1-83948353de4d.png)
![2](https://user-images.githubusercontent.com/26890946/167965368-21261a46-9a11-4183-8a9b-d15e20be94c4.png)
![3](https://user-images.githubusercontent.com/26890946/167965394-b59751c5-42d1-4529-8f40-0c946b254ed0.png)
![4](https://user-images.githubusercontent.com/26890946/167965403-79851499-8334-4a56-bb45-8721aaed2862.png)


# Chapter 2, Day 3:

## Quests

1.
<img width="572" alt="2 3, q1" src="https://user-images.githubusercontent.com/26890946/168696923-5e58dd49-32c5-4110-9070-79578fcfb5a1.png">

2.
<img width="939" alt="2 3, q2" src="https://user-images.githubusercontent.com/26890946/168696701-a9ef8a04-ab0c-491a-b80f-4c5b488b4e04.png">


3. The force-unwrap operator "!" unwraps the optional type, allowing us to find out if it is/isn't nil

4. The error in the image means that an optional has been returned when attempting to access the value of address 0x03, meaning it may be nil! The way to fix this is to use the force unwrap operator [!] when returning 0x03:
<img width="671" alt="2 3, q4" src="https://user-images.githubusercontent.com/26890946/168696787-36e8081b-7655-49e1-a5d6-87fb1ecea8bb.png">



# Chapter 2, Day 4:

## Quests

1 & 2. 
<img width="705" alt="2 4 Q1-2" src="https://user-images.githubusercontent.com/26890946/168997032-de2e550e-a79a-4b5d-8e68-10d7c68cf628.png">

3.
<img width="972" alt="2 4 Q3" src="https://user-images.githubusercontent.com/26890946/168997058-30106c98-f91b-482d-9359-4d4abb96a423.png">

4.
<img width="1303" alt="2 4 Q4" src="https://user-images.githubusercontent.com/26890946/168997067-eed719db-127a-4fc5-82a2-3fd392f5f2ce.png">



# Chapter 3, Day 1:

## Quests

1. While similar to Structs in that they are both "containers of data", Resources cannot be overwritten or copied, and thus, are much more secure. 

2. We may find it preferable to use Resources over Structs when, for example, we need to make a high value transaction (or, commonly in this space: send an NFT). This is an instance in which security would be considered paramount, and Resources are extremely difficult to lose. 

3. The "Create" keyword is used inside a contract to make a new Resource.

4. Resources can only ever be made inside of Contracts; never in Scripts or Transactions. 

5. The type of resource displayed in the example is a String.

6. 4 Errors in the provided code:
	1. @ symbol (required to missing next to Jacob where: 
			  
        pub fun createJacob(): Jacob

	2. there are two errors where:

			let myJacob = Jacob() 

    a.) we create a new "Jacob" type by using the create keyword 
    b.) the equal sign should be replaced by the move operator ( <- ), which must be used to move resources around
    
  3. where:
       
    return myJacob
 
   we are missing a move operator ( <- ) between return and myJacob.

