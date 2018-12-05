**Note: THE FILECOIN PROJECT IS STILL EXTREMELY CONFIDENTIAL. Do not share or discuss the project outside of designated preview channels (chat channels, Discourse forum, GitHub, emails to Filecoin team), not even with partners/spouses/family members. If you have any questions, please email [legal@protocol.ai](mailto:legal@protocol.ai).**

# Filecoin sample data

Learn how to store and retrieve data on Filecoin using the sample data in this repository.

All files in this folder are covered under Creative Commons (CC) licenses that allow data to be used for commercial purposes and to be reused with modification.

## Storing data in Filecoin

```Shell
cd $GOPATH/src/github.com/filecoin-project/go-filecoin

// Import image from sample data; returns content identifier 
// <CID>
go-filecoin client import path/to/sample-data/camel.jpg

// Find a storage miner whose ask meets your needs
go-filecoin orderbook asks | jq

// Propose storage deal. Find <miner address> from the ask. 
// If the deal is accepted, you will see a return value like 
// "Status: accepted". Note that duration here is in number of 
// blocks (each block takes 30s to produce).
go-filecoin client propose-storage-deal <miner address> <CID> <duration> --price=<price>
```

For more documentation on how to use Filecoin, go to the [go-filecoin wiki](https://github.com/filecoin-project/go-filecoin/wiki).

## Data in this folder

`angry-cat.jpg`<br />
![Angry cat](/angry-cat.jpg)

`baby-elephant.jpg`<br />
![Baby elephant](/baby-elephant.jpg)

`camel.jpg`<br />
![Camel](/camel.jpg)

`corgi.jpg`<br />
![Corgi](/corgi.jpg)

`dolan.png`<br />
![Dolan](/dolan.png)

`dolphin.jpg`<br />
![Dolphin](/dolphin.jpg)

`happy-puppy.jpg`<br />
![Happy puppy](/happy-puppy.jpg)

`invictus.txt`<br />
```
"Invictus" 
by William Ernest Henley


Out of the night that covers me, 
      Black as the pit from pole to pole, 
I thank whatever gods may be 
      For my unconquerable soul. 

In the fell clutch of circumstance 
      I have not winced nor cried aloud. 
Under the bludgeonings of chance 
      My head is bloody, but unbowed. 

Beyond this place of wrath and tears 
      Looms but the Horror of the shade, 
And yet the menace of the years 
      Finds and shall find me unafraid. 

It matters not how strait the gate, 
      How charged with punishments the scroll, 
I am the master of my fate, 
      I am the captain of my soul. 
```

`kitten.jpg`<br />
![Kitten](/kitten.jpg)

`krakow-animated.jpg`<br />
![Krakow animated](/krakow-animated.jpg)

`lemur.jpg`<br />
![Lemur](/lemur.jpg)

`nasa-andromeda.jpg`<br />
![Andromeda](/nasa-andromeda.jpg)

`nasa-coronas-black-holes.jpg`<br />
![Coronas/Black holes](/nasa-coronas-black-holes.jpg)

`nasa-earth.jpg`<br />
![Earth](/nasa-earth.jpg)

`nasa-high-energy-x-rays.jpg`<br />
![High energy X-rays](/nasa-high-energy-x-rays.jpg)

`neurotic-puppy.jpg`<br />
![Neurotic puppy](/neurotic-puppy.jpg)

`panda-hug.jpg`<br />
![Pandas hugging](/panda-hug.jpg)

`puppy.jpg`<br />
![Puppy](/puppy.jpg)

`rotating-earth.gif`<br />
![Rotating Earth](/rotating-earth.gif)

`sick-shel-silverstein.txt`<br />
```
"Sick"
by Shel Silverstein

“I cannot go to school today,"
Said little Peggy Ann McKay.
“I have the measles and the mumps,
A gash, a rash and purple bumps.
My mouth is wet, my throat is dry,
I’m going blind in my right eye.
My tonsils are as big as rocks,
I’ve counted sixteen chicken pox
And there’s one more—that’s seventeen,
And don’t you think my face looks green?
My leg is cut—my eyes are blue—
It might be instamatic flu.
I cough and sneeze and gasp and choke,
I’m sure that my left leg is broke—
My hip hurts when I move my chin,
My belly button’s caving in,
My back is wrenched, my ankle’s sprained,
My ‘pendix pains each time it rains.
My nose is cold, my toes are numb.
I have a sliver in my thumb.
My neck is stiff, my voice is weak,
I hardly whisper when I speak.
My tongue is filling up my mouth,
I think my hair is falling out.
My elbow’s bent, my spine ain’t straight,
My temperature is one-o-eight.
My brain is shrunk, I cannot hear,
There is a hole inside my ear.
I have a hangnail, and my heart is—what?
What’s that? What’s that you say?
You say today is. . .Saturday?
G’bye, I’m going out to play!”
```

`swiral-testav.gif`<br />
![Swiral Testav](/swiral-testav.gif)

`woke-puppy.jpg`<br />
![Woke puppy](/woke-puppy.jpg)

## License

The Filecoin Project is dual-licensed under Apache 2.0 and MIT terms:

- Apache License, Version 2.0, ([LICENSE-APACHE](https://github.com/filecoin-project/sample-data/blob/cleanup/LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](https://github.com/filecoin-project/sample-data/blob/cleanup/LICENSE-MIT) or http://opensource.org/licenses/MIT)
