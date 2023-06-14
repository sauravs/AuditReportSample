

# WEB3Tech_HappyGeeks

 Set of smart contracts for minting  20 sets of unique NFT characters


---
**Code Repo Link** :  https://github.com/agarwalankit3395/ExclusiveCollection
---

---
<ins>**Product Description**<ins>

Limited Edition NFT is 20 Exclusive NFTs with a set of 25 copies each. User can claim only one NFT free of cost. 
Initally user need not to pay anything to claim these NFTs. When user sell them on marketplace like Opensea, 10% royalty will be deducted and given to WEB3Tech_HappyGeeks Contract Owner

 ---

<ins>**Steps to follow to execute the code**<ins>

## Installation

After downloading  or cloning the repo, initialize an ` npm ` project run
```
npm install
```
Once it's installed, just run the follwing command and follow its instructions:

```
Change the `.env.sample` into `.env`
```
Update the APIs in ```.env``` files
```
PRIVATE_KEY=<ADD_YOUR_PRIVATE_KEY_HERE>
POLYGONSCAN_API_KEY=<ADD_YOUR_POLYGON_API_HERE>
POLYGON_MAINNET_URL=https://polygon-mainnet.g.alchemy.com/v2/<ADD_YOUR_API_HERE>
POLYGON_TESTNET_URL=https://polygon-mumbai.g.alchemy.com/v2/<ADD_YOUR_API_HERE>
```

Compile the Smart Contract :  
```
npx hardhat compile
```
Deploy the smart contract on polygon testnet :  
``` 
npx hardhat run .\scripts\deploy-happytime.js --network polygonMumbai
```
Update the `SMART_CONTRACT_ADDRESS` and then Verify the smart contract on polygon testnet : 
```
npx hardhat verify --network polygonMumbai SMART_CONTRACT_ADDRESS
```


---

<ins>**As per Initial Audit Consultation Questionnaire Response provided by Client**<ins>

| **SNo** | **Questions**                                                                                                                                                      | **Client's Response**                                                                                                                                                                                                                                   |
|---------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1       | Client/Organisation Name                                                                                                                                           | Ankit Agarwal                                                                                                                                                                                                                                           |
| 2       | Email                                                                                                                                                              | agarwalankit3395@gmail.com                                                                                                                                                                                                                              |
| 3       | If you have a public code repo, please share it here                                                                                                               | https://github.com/agarwalankit3395/ExclusiveCollection/tree/main                                                                                                                                                                                       |
| 4       |  How many contracts are in scope?                                                                                                                                  | One (WEB3Tech_HappyGeeks.sol)                                                                                                                                                                                                                           |
| 5       |  How many external imports are there?                                                                                                                              | Two                                                                                                                                                                                                                                                     |
| 6       | How many separate interfaces and struct definitions are there for the contracts within scope?                                                                      |  None                                                                                                                                                                                                                                                   |
| 7       | Does most of your code generally use composition or inheritance?                                                                                                   | Inheritance                                                                                                                                                                                                                                             |
| 8       | How many external calls?                                                                                                                                           | 8                                                                                                                                                                                                                                                       |
| 9       | Are automated test cases provided?                                                                                                                                 | No                                                                                                                                                                                                                                                      |
| 10      |  Test Coverage Percentage?                                                                                                                                         | 0%                                                                                                                                                                                                                                                      |
| 11      | Does Automated Tests cases include integration test, or unit test, or both?                                                                                        | None                                                                                                                                                                                                                                                    |
| 12      |  Is there a need to understand a separate part of the codebase / get context in order to audit this part of the protocol? If so, please describe required context: | Is a ERC1155 Contract with ERC2981 which is a royalty standard. Basically, Some limited edition of NFT need to be minted between Id 1 to 20 and 25 copies of each. One wallet who trigger the transaction can mint only one NFT from enitre collection. |
| 13      | Does it use an oracle? If so, explain briefly.                                                                                                                     | No                                                                                                                                                                                                                                                      |
| 14      | Does the token confirm to the ERC20 standard?                                                                                                                      | No, Its a NFT Contract with ERC721 standard from Openzeppelin.                                                                                                                                                                                          |
| 15      | Which category your smart contract business logic generally falls into?                                                                                            | NFT                                                                                                                                                                                                                                                     |
| 16      | Is it a fork of a popular project? If so, provide link of that forked project                                                                                      | No                                                                                                                                                                                                                                                      |
| 17      | Does it use rollups?                                                                                                                                               | No                                                                                                                                                                                                                                                      |
| 18      | Is it multi-chain?                                                                                                                                                 | No                                                                                                                                                                                                                                                      |
| 19      | Does it use a side-chain?                                                                                                                                          | No                                                                                                                                                                                                                                                      |
| 20      | Total no. of lines in the scope of the audit?                                                                                                                      | 90                                                                                                                                                                                                                                                      |
| 21      | "                                                                                                                                                                  |
|         |   Which Tier auditing are you looking for or interested in? Please read more on our website related to our different Tier levels.                                  |
|         |   (Note: We do not support Tier-I Audit ,if you do not have automated testcases ,or test coverage more than 70%)"                                                  | Tier I                                                                                                                                                                                                                                                  |
| 22      | Any common automated auditing tool you run? If yes, request you to let us know the tools.                                                                          | No                                                                                                                                                                                                                                                      |
| 23      | Request you to provide your preferred contact information via which we should contact you back. It could be email, phone, discord, telegram, skype or other.       | ankit.agarwal@pridevel.com                                                                                                                                                                                                                              |
| 24      | Request you to let us know your preferred date and time for Step 2. We will share with you a meeting link at date and time.                                        | 13th Jun , 4-5 PM                                                                                                                                                                                                                                       |
| 25      | Request you to provide your Polygon chain Wallet Address for the purpose of receiving NFT certificate.                                                             | 0x911783781755C7A8cE91898C6E19ee057ba94dB6                                                                                                                                                                                                              |
                                                          |
---



## Initial Auditing Report Summary<ins>

 
 | **SNo** | **Title**                                   | **Response**                |
|---------|---------------------------------------------|-----------------------------|
| 1       | No. Of Major Issue Found                    | 0                           |
| 2       | No. Of. Medium Risk Issue Found             | 0                           |
| 3       | No. Of. Low Risk/Non-Critical Issue Found   | 3                           |
| 4       | Gas Optimization Related Issue Found        | 5                           |
| 5       | Is Automated Test Coverage Provided         | No                          |
| 6       | No of Checkpoints Covered                   | 104                         |
| 7       |  No of Checkpoints Skipped                  | 27                          |
| 8       | No of Checkpoints Not Applicable            | 22                          |
| 9       | Auditor Name                                | Saurav Shekhar              |
| 10      | Auditing Date                               | 9th June - 12th June , 2023 |
| 11      | Audit Type                                  | Tier- III                   |
| 12      | Total no of lines of code in scope of Audit | 90                          |
| 13      |  No. of hours Taken To Audit                | 12-15                       |

 
 ---



 ## <ins>GAS OPTIMIZATION RELATED ISSUES DETAILS<ins>
 
 

 >**PVL-2:** <ins>array[index] += amount is cheaper than array[index] = array[index] + amount <ins>
 
 **ISSUE_TYPE:**  GAS OPTIMIZATION
 
  **Description:**  When updating a value in an array with arithmetic, using array[index] += amount is cheaper than array[index] = array[index] + amount.
  This is because you avoid an additional mload when the array is stored in memory, and an sload when the array is stored in storage.  
   This can be applied for any arithmetic operation including +=, -=,/=,*=,^=,&=, %=, <<=,>>=, and >>>=.   
   
   This optimization can be particularly significant if the pattern occurs during a loop.
   
   ```javascript
   
   //Unoptimized
   idRecord[id] = idRecord[id]+perUser;   // Execution Cost : 24942
   
   //Optimized
   
   idRecord[id] += perUser;    // Execution Cost : 24877
   
   ```
   
 **File Name:** https://github.com/agarwalankit3395/ExclusiveCollection/blob/main/contracts/Happyniess.sol
 
 **Line No:** 59
 
 **No. Of Instances:** 1
   
 **Reported By:** Saurav Shekhar

 **Accepted/Rejected By:** Ankit Agarwal
 
 **Accepted:** YES
   
 **If not Accepted,please state the reason:**  NA
   
   
   
>**PVL-12:** <ins>Use Custom Errors<ins>

**ISSUE_TYPE:**  GAS OPTIMIZATION
	
**Description:** Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

```javascript
   
//Unoptimized:

function add(uint256 _amount) public {
	require(msg.sender == owner, "unauthorized");
	total += _amount;
}


//Optimized:

error Unauthorized(address caller);

function add(uint256 _amount) public {
	if (msg.sender != owner)
    	revert Unauthorized(msg.sender);

	total += _amount;
}

```
	
	
	
   
**File Name:** https://github.com/agarwalankit3395/ExclusiveCollection/blob/main/contracts/Happyniess.sol
 
 **Line No:**   54,55,56,72 ,77 ,78 
 
 **No. Of Instances:** 6
   
  **Reported By:** Saurav Shekhar

 **Accepted/Rejected By:** Ankit Agarwal
 
 **Accepted:** NO
   
 **If not Accepted,please state the reason:** Custom error works only in case if we are reverting with if statement.In this case ,its not applicable

   
   
   
>**PVL-25:** <ins> Optimized packing of storage variables <ins>
	
**ISSUE_TYPE:** GAS OPTIMIZATION
	
**Description:**
	 In ethereum, you pay gas for every storage slot you use. A slot is of 256 bits, and you can pack as many variables as you want in it.
	Packing is done by solidity compiler and optimizer automatically, you just need to declare the packable functions consecutively.
	The below code is an example of poor code and will consume 3 storage slot
	This small change will save you a lot of gas as it will now only need 2 slots to store 
   (It takes 20k gas to store 1 slot of data).

```javascript

uint8 numberOne;
uint256 bigNumber;
uint8 numberTwo;

//A much more efficient way to do this in solidity will be:

uint8 numberOne;
uint8 numberTwo;
uint256 bigNumber;

```

   
 File Name: https://github.com/agarwalankit3395/ExclusiveCollection/blob/main/contracts/Happyniess.sol
 
**Line No:**   16,17,18,19
 
**No. Of Instances:**  4
   
**Reported By:** Saurav Shekhar

**Accepted/Rejected By:** Ankit Agarwal
 
**Accepted:** YES
   
**If not Accepted,please state the reason:**  NA
 
   
   
   
>**PVL-28:**  <ins>Use unchecked for arithmetic where you are sure it won't over or underflow<ins>
	
**ISSUE_TYPE:** GAS OPTIMIZATION
	
**Description:**
	In the example below, the variable i cannot overflow because of the condition i < length, where length is defined as uint256.
    The maximum value i can reach is max(uint)-1. Thus, incrementing i inside an unchecked block is safe and consumes less gas.

```javascript
function loop(uint256 length) public {
      	for (uint256 i = 0; i < length; ) {
        	// do something
       	unchecked {
        	i++;
        	}
      	}
     	}

```
**File Name:** https://github.com/agarwalankit3395/ExclusiveCollection/blob/main/contracts/Happyniess.sol
 
**Line No:** 84
 
**No. Of Instances:** 1
   
**Reported By:**  Saurav Shekhar
   
**Accepted/Rejected By:**  Ankit Agarwal
   
**Accepted:** YES
   
**If not Accepted,please state the reason:** NA
   
 
 
>**PVL-46:**  <ins>Use separate checks in require() to save gas<ins>
  
**ISSUE_TYPE:** GAS OPTIMIZATION
	
**Description:**      
This will cost more to deploy, but can save gas when the function is run.
This can be useful if you know a function in your smart contract will be called many times that it can justify the larger deploy cost.   

```javascript
	
	// Unoptimized 
	
	 / 229,940 gas to deploy
pragma solidity >=0.8.4;

contract UnoptimizedVersion {
	mapping(address => uint256) balances;
	bool isActive = true;

	constructor() {
    	balances[msg.sender] = 999;
	}

	// 29,622 gas to run
	function Unoptimized() external payable returns (uint) {
    	require(isActive && balances[msg.sender] > 0 && msg.value > 0, "errmsg");

    	return 1;
	}
}




   // Optimized
   
   
   pragma solidity >=0.8.4;

// 309,456 gas to deploy
contract OptimizedVersion {
	mapping(address => uint256) balances;
	bool isActive = true;

	constructor() {
    	balances[msg.sender] = 999;
	}

	// 29,604 gas to run
	function Optimized() external payable returns (uint) {
    	require(isActive, "errMsg");
    	require(balances[msg.sender] > 0 , "errMsg2");
    	require(msg.value > 0, "errmsg");

    	return 1;
	}
}

```
	

**File Name:** https://github.com/agarwalankit3395/ExclusiveCollection/blob/main/contracts/Happyniess.sol
 
**Line No:** 54,72
 
**No. Of Instances:** 2
   
 **Reported By:**  Saurav Shekhar
   
**Accepted/Rejected By:**  Ankit Agarwal
   
**Accepted:** Yes
   
**If not Accepted,please state the reason:** NA
   
 

---

## <ins>Non-Critical/Low-Risk/Quality-Assurance Related Issues<ins>
 
 
 >**PVL-63:** <ins>Avoid Use of floating Pragma<ins>
	
**ISSUE_TYPE:**  NON-CRITICAL/LOW RISK / QUALITY ASSURANCE
	
**Description:**
Contracts should be deployed with the same compiler version and flags that they have been tested with thoroughly.
	Locking the pragma helps to ensure that contracts do not accidentally get deployed using, for example,an outdated compiler version 
	that might introduce bugs that affect the contract system negatively.

   
**File Name:** https://github.com/agarwalankit3395/ExclusiveCollection/blob/main/contracts/Happyniess.sol
 
**Line No:** 2
 
**No. Of Instances:** 1
   
  
 **Reported By:**  Saurav Shekhar
   
**Accepted/Rejected By:**  Ankit Agarwal
   
**Accepted:** YES
   
**If not Accepted,please state the reason:** NA
   
 
 
>**PVL-115:** <ins>Insufficient test coverage<ins>
	
**ISSUE_TYPE:**  NON-CRITICAL/LOW RISK / QUALITY ASSURANCE
	
**Description:** Check for total test coverage for the contracts.It should be more than 80%
	
  
 **Reported By:**  Saurav Shekhar
   
**Accepted/Rejected By:**  Ankit Agarwal
   
**Accepted:** NO
   
**If not Accepted,please state the reason:** Not intended to write test cases for this project due to time constraint
   
 
>**PVL-119:** <ins>Do proper commenting and include return parameters in NatSpec comments<ins>
	
**ISSUE_TYPE:**  NON-CRITICAL/LOW RISK / QUALITY ASSURANCE
	
**Description:** It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI).
It is clearly stated in the Solidity official documentation.
In complex projects such as Defi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.   
    
 **Reported By:**  Saurav Shekhar
   
**Accepted/Rejected By:**  Ankit Agarwal
   
**Accepted:** YES
   
**If not Accepted,please state the reason:** NA
   
 
 
 
