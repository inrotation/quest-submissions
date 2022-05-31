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
3. In the _Prepare_ phase of a transaction, we are accessing data in someone’s account, while in the _Execute_ phase we are changing some data![Q4D2, d](https://user-images.githubusercontent.com/26890946/170925065-4a5745dc-c247-4d15-a84a-000b16156173.png)

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
1.

<img width="439" alt="Q3D2" src="https://user-images.githubusercontent.com/26890946/170593292-bdbaa592-bb67-4dd9-b006-ee0e1c00d365.png">

# Chapter 3, Day 3
## Quests

1.

<img width="482" alt="Q3D3, 1" src="https://user-images.githubusercontent.com/26890946/170596560-b0195fc4-b0df-4b89-bb2d-79350d68e4fe.png">

2.

<img width="446" alt="Q3D3, 2" src="https://user-images.githubusercontent.com/26890946/170596652-9c8479f4-eb89-4ccc-86d9-cf858b03a325.png">

3. In Cadence, References can be especially useful when there's a desire to glean information from or interact with some data (usually Structs or Resources) without the laborious task of being forced to hold/move onto said data. 



# Chapter 3, Day 4
## Quests

1.  Interfaces specify a set of requirements for something to implement and can allow for only certain things to be exposed to people.
2. 
	
	Example 1

	<img width="447" alt="Q3D4, 2 1" src="https://user-images.githubusercontent.com/26890946/170795566-2d8729fc-80ea-471e-974a-84b7dac9de38.png">

	Example 2
	
	<img width="756" alt="Q3D4, 2 2" src="https://user-images.githubusercontent.com/26890946/170795583-c14bba3a-44ae-47b4-a8b5-7d98cd5d7311.png">  

  
  
3. Code fixes included with comments: 
	<img width="550" alt="Q3D4, 3" src="https://user-images.githubusercontent.com/26890946/170895281-0d05df6c-1efd-4fde-aacf-0b1eacfaf53a.png">



# Chapter 3, Day 5
## Quests

***Area 1***

a) 	read & write  
b) 	read & write       
c) 	read & write      
d) 	read & write     

publicFunc - can be called  
contractFunc - can be called  
privateFunc - can be called  


***Area 2***

a) 	read & write  
b) 	read, no write   
c) 	read, no write  
d) 	no read, no write 

publicFunc - can be called  
contractFunc - can be called  
privateFunc - cannot be called 


***Area 3***

a) 	read & write  
b) 	read & write  
c) 	read, no write  
d) 	no read, no write  

publicFunc - can be called  
contractFunc - can be called  
privateFunc - cannot be called  

***Area 4***

a) 	read & write  
b) 	read, no write   
c) 	no read, no write     
d) 	no read, no write    

publicFunc - can be called  
contractFunc - cannot be called  
privateFunc - cannot be called  

# Chapter 4, Day 1
## Quests

1. Contract Code and Account Storage (where data is stored) reside in every Flow account.  

2. The following paths reside in the Account Storage portion of Flow accounts; however, they differ in that:
	/storage/ - is only accessible by the account owner; all data resides here
	/public/  - data placed here is available to everybody
	/private/ - is only accessible to account owner & people (s)he gives access to 

3.  The .save() function is used to save something to Account Storage  
	The .load() function is used in order to remove data  
	The .borrow() function is used so as to look at something within an account

4. We couldn't save something to our account storage inside of a script because we read (and not change) data within a Script

5. As only the account holder has authorization, you would not be able to to save something to my account.

6. 
	Contract:
	
	<img width="404" alt="Q4D1, 6 contract" src="https://user-images.githubusercontent.com/26890946/170889384-5960894e-68fd-4b7e-b9d2-dc6c30be73e0.png">

	Saves Resource:
	<img width="621" alt="Q4D1, 6 Save" src="https://user-images.githubusercontent.com/26890946/170891276-79c0562c-799e-4bef-bb08-4106a0b5b4e9.png">

	
	Loads/Destroys Resource:
	<img width="815" alt="Q4D1, 6 load" src="https://user-images.githubusercontent.com/26890946/170891280-acee3638-73b4-44b4-9bee-14779063704d.png">

	Borrows Resource:

	<img width="666" alt="Q4D1, 6 borrow" src="https://user-images.githubusercontent.com/26890946/170891289-4d861304-3789-46b0-b242-30427e7e951c.png">


# Chapter 4, Day 2
## Quests

1. .link() is used to link our resource from the /storage/ path to the /public/ path, thus making it publically accessible  

2. We can use resource interfaces to only expose certain things to the /public/ path by using discretion in making only those specific things in the /storage/ path publically available.  

3. 
![Q4D2, a](https://user-images.githubusercontent.com/26890946/170922109-67994a0d-b82d-4cb9-81ae-233415c5f829.png)

![Q4D2, b](https://user-images.githubusercontent.com/26890946/170922143-9b019e7d-a561-4987-af55-f0c5a258e690.png)

![Q4D2, c](https://user-images.githubusercontent.com/26890946/170923085-21deb932-1848-4b35-b238-410cc929f49f.png)

![Q4D2, d](https://user-images.githubusercontent.com/26890946/170925098-790c98ff-3553-44ac-99e1-536716c4bd2c.png)


# Chapter 4, Day 3
## Quests

1. We added a Collection to this contract in order to fix the problem of storing more than one NFT to our account without having to specify a new storage path every time. Additionally, it allows for more than only the account owner to store an NFT in his/her storage account. 
2. The Cadence language requires a destroy function to be implemented so as to delete  "nested resources" (resources inside of resources).
3. Something to consider adding is some Resource that will restrict mint access to holders. Also, a Borrow function inside the Collection would allow us to read the NFT without needing to remove it. 


# Chapter 4, Day 4
## Quests

<img width="776" alt="Q4D4, 1" src="https://user-images.githubusercontent.com/26890946/171302282-3f2b8829-64d9-4288-bbc1-29eea7d0a394.png">
<img width="625" alt="Q4D4, 2" src="https://user-images.githubusercontent.com/26890946/171302290-f77cb786-acf4-4e64-94cd-8b5ea4d7f4cd.png">


# Chapter 5, Day 1
## Quests

	
