const NFTs = [];


const mintNFT = function (_name, _color, _music, _artist) {
  const NFT = {
    name: _name,
    color: _color,
    music: _music,
    artist: _artist,
  };

  NFTs.push(NFT);

  console.log(`Congratulations! Your NFT "${NFT.name}" has been minted successfully.\n`);
};

const printNFTs = function () {
  console.log("All NFTs:\n");

  for (let i = 0; i < NFTs.length; i++) {
    console.log(`ID: ${i + 1}`);
    console.log(`Name: ${NFTs[i].name}`);
    console.log(`Color: ${NFTs[i].color}`);
    console.log(`music: ${NFTs[i].music}`);
    console.log(`artist: ${NFTs[i].artist}\n`);
  }

  console.log("Finished printing all NFTs.\n");
};


const getTotalSupply = function () {
  console.log(`Total number of minted NFTs: ${NFTs.length}`);
};


mintNFT("M1", "orange", "closer", "The_Chainsmokers");
mintNFT("M2", "Black", "hurricane", "martin_garix");
mintNFT("M3", "yellow", "lonely", "akon");
mintNFT("M4", "teal", "bones", "imagine_dragons");


printNFTs();


getTotalSupply();



