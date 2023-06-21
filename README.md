# JavaScript-Assessment-Metacrafters
/*
Assessment Requirements
1. Create a variable that can hold a number of NFT's. What type of variable might this be?
2. Create an object inside your mintNFT function that will hold the metadata for your NFTs. 
   The metadata values will be passed to the function as parameters. When the NFT is ready, 
   you will store it in the variable you created in step 1
3. Your listNFTs() function will print all of your NFTs metadata to the console (i.e. console.log("Name: " + someNFT.name))
4. For good measure, getTotalSupply() should return the number of NFT's you have created
*/

// create a variable to hold your NFT's
   const NftNum =[];

// this function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT ( _name,_ShirtSize, _ShirtColor,_bling){
   const NFTobj ={
      "name":_name,
      "ShirtSize" :_ShirtSize,
      "ShirtColor" :_ShirtColor,
      "bling" :_bling
   };
   NftNum.push(NFTobj);
   console.log("Minted :" +_name);
}
// create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()
function listNFTs () {
   for(let i=0; i<NftNum.length; i++){
      console.log("\nID: \t\t" +(i +1));
      console.log("Name: \t\t" + NftNum[i].name);
      console.log("Shirt Size: \t" + NftNum[i].ShirtSize);
      console.log("Shirt Color: \t" + NftNum[i].ShirtColor);
      console.log("Shirt Size: \t" + NftNum[i].ShirtSize);
      console.log("Bling: \t\t" + NftNum[i].bling);
   }
}
// print the total number of NFTs we have minted to the console
function getTotalSupply() {
   console.log("\n Total no of NFTs We have :" +NftNum.length);
}

// call your functions below this line
mintNFT("Nike","M","Blue","Silver Plated");
mintNFT("Tommy","S","Pink","Gold Plated");
mintNFT("Zara","M","Green","Plain");
mintNFT("Jokey","M","Blue","Silver Plated");
mintNFT("u.s polo","xl","Red","Plain");
mintNFT("Netplay","M","Blue","Silver Plated");
listNFTs();
getTotalSupply();

output 
[Running] node "/workspace/Beginning-Javascript/playground.js"
Minted :Nike
Minted :Tommy
Minted :Zara
Minted :Jokey
Minted :u.s polo
Minted :Netplay

ID: 		1
Name: 		Nike
Shirt Size: 	M
Shirt Color: 	Blue
Shirt Size: 	M
Bling: 		Silver Plated

ID: 		2
Name: 		Tommy
Shirt Size: 	S
Shirt Color: 	Pink
Shirt Size: 	S
Bling: 		Gold Plated

ID: 		3
Name: 		Zara
Shirt Size: 	M
Shirt Color: 	Green
Shirt Size: 	M
Bling: 		Plain

ID: 		4
Name: 		Jokey
Shirt Size: 	M
Shirt Color: 	Blue
Shirt Size: 	M
Bling: 		Silver Plated

ID: 		5
Name: 		u.s polo
Shirt Size: 	xl
Shirt Color: 	Red
Shirt Size: 	xl
Bling: 		Plain

ID: 		6
Name: 		Netplay
Shirt Size: 	M
Shirt Color: 	Blue
Shirt Size: 	M
Bling: 		Silver Plated

 Total no of NFTs We have :6

[Done] exited with code=0 in 0.042 seconds






