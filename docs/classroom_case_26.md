## micro:coin

Have you heard about BitCoin and all those new Crypto currencies? Well micro:bit has micro:coin now!

### How does a micro:bit make coins?

Each micro:bit contains a **block chain**, a sequence of **blocks**, that is public and can’t be modified. Each block represents a **coin**. To mine new coins, the user shakes the micro:bit and, if they are in luck, their coin added to the chain as a new block! Once the block is added, it is broadcasted to the other micro:bit (the block chain is public and can’t be modified so it’s ok to share it). Other micro:bits receive the block, validate the transaction and update their block chain as needed.

Pressing `A` shows the number of block you added to the chain, that’s your score. Pressing `B` shows you the length of the chain.

Happy mining!

### Coins, blocks, chains

A *block chain* is a list of blocks that record transactions of a crypto-currency like BitCoin. A block might contain information like the time it was created (mined) and who mined it. The most important part of the block is it’s hash. This is a special number made from the information in the last block of the block list combined with the hash number of previous block in the list. The new block contains information for the current transaction and this new hash number. The new block is added to the list of previous blocks. This list is then transmitted to the crypto currency network. It’s really hard (like impossible) to tamper or forge a hash which allows the block chain to be transmitted publically.

Build yourself a micro:bit wallet to hold your coins!

### Code

The code uses blocks from radio-blockchain package.

- Click on **Advanced**, then **Add Package**
- Search for **blockchain** and add **radio-blockchain**

![](https://i.imgur.com/kaFwqGH.png)

Link: [https://makecode.microbit.org/_H3zRH9RA7JTM](https://makecode.microbit.org/_H3zRH9RA7JTM)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_H3zRH9RA7JTM" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### How does the blockchain code work?

The [radio-blockchain](https://makecode.microbit.org/pkg/microsoft/pxt-radio-blockchain) package uses radio to transmit blocks between micro:bits. You can see how this package works by reading the JavaScript sources at [https://github.com/microsoft/pxt-radio-blockchain](https://github.com/microsoft/pxt-radio-blockchain). To go right to the blockchain code, see this file:

[main.ts ](https://github.com/Microsoft/pxt-radio-blockchain/blob/master/main.ts)- contains the complete JavaScript source for the blockhain. Have a good read!

