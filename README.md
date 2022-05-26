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

4.1
	
<img width="420" alt="1" src="https://user-images.githubusercontent.com/26890946/170377906-da77d06a-3173-4564-8ac1-5f1dee14ea53.png">

4.2
	
<img width="433" alt="2" src="https://user-images.githubusercontent.com/26890946/170377957-2a0809d7-b701-445a-bcf5-c83b7800def9.png">

4.3
	
<img width="473" alt="3" src="https://user-images.githubusercontent.com/26890946/170377996-91f75609-c63a-45d6-8efb-41105172f5dc.png">

4.4
	
<img width="430" alt="4" src="https://user-images.githubusercontent.com/26890946/170378009-7ef74873-9421-4143-b9eb-76da3587b5dd.png">




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

1-3.

<img width="786" alt="Q2 4, 1-3" src="https://user-images.githubusercontent.com/26890946/170580297-662279b7-d918-4c5c-bbcb-408757cac495.png">


4.

<img width="730" alt="Q2 4, 4" src="https://user-images.githubusercontent.com/26890946/170581009-1d6faa24-46ab-4eb9-b457-db159ccca47f.png">


5.

<img width="1114" alt="Q2 4, 5" src="https://user-images.githubusercontent.com/26890946/170581749-729f58b8-3144-4693-84f9-c61052a33484.png">



# Chapter 3, Day 1:

## Quests

1. While similar to Structs in that they are both "containers of data", Resources cannot be overwritten or copied, and thus, are much more secure. 

2. We may find it preferable to use Resources over Structs when, for example, we need to make a high value transaction (example: send an NFT). This is an instance in which security would be considered paramount, and Resources are extremely difficult to lose. 

3. The "Create" keyword is used inside a contract to make a new Resource.

4. Resources can only ever be made inside of Contracts; never in Scripts or Transactions. 

5. The type of resource displayed in the example is a String.

6. The 4 Errors in the provided code:

	I.) The @ symbol is missing next to Jacob, where: 
			  
        	pub fun createJacob(): Jacob


	II.) There are two errors where:

			let myJacob = Jacob() 

	a. We create a new "Jacob" type by using the create keyword; it is missing here. 
    	
	b. The equal sign should be replaced by the move operator (<-), which must be used to move resources around
	
	
	III.) Where:
       
       	return myJacob
 	
	We are missing a move operator ( <- ) between return and myJacob.
	

# Chapter 3, Day 2:

## Quests

<img width="439" alt="Q3D2" src="https://user-images.githubusercontent.com/26890946/170593292-bdbaa592-bb67-4dd9-b006-ee0e1c00d365.png">



