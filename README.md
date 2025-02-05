# GOSQAS Demo

This is experimental code for the [GOSQAS project](https://github.com/gosqas/home/blob/main/README.md).

GOSQAS is grateful to @devhawk (Harry Pierson) for rapidly protoyping this demo.

## A Live MVP

We are developing a Minimal Viable Product. Although still a work in progress, you can try it out here:

[https://gosqas.org/](https://gosqas.org/)

## Installation

Clone the repo, and then execute:
```
> npm install
> npm run dev
```

Then point your browser at [http:\\localhost:8000](http:\\localhost:8000) for example.

> Note, as of v0.2, the demo server listens on *all* networks the server is connected to.
> While exposing server ports is always a security risk, exposing the demo server on the local network
> allows other devices - mobile devices in particular - to access the demo server.
> On startup, the server prints out a list of the IP addresses it is listening on.

## Video of Operation

We have made a [short video](https://youtu.be/E5_YQV72NyY) of [v0.1](https://github.com/gosqas/asset-provenance-tracking/releases/tag/v0.1) operation.

## batch-shell.sh

The file batch-shell.sh can be used to produce any number of keys and QR codes at at ime.
It takes a single argument, the number N of keys and QR codes to create. It will
populate the current directory directly with N files, each of which has the name of a device key, and whose
body a .png file of the QR code that resolves to that key. An internal variable defines the full URL.
The name in the start record is currenlty hard-coded to "MakerFaireBayArea" but can of course be changed.

This can be executed with:

```
> batch-shell.sh 300
```
for example, to generate 300 valid QR codes.

## A Note on Our Trademarks

Although all of our code is open-source, you may not user our trademarkes without written permission.
Our trademarks include:
1. The word GOSQAS
2. The term "Global Open Source Quality Assurance System"
3. The "purple hands" logo
4. The word-ard GOSQAS with the "purple hands" symbol in the letter O.
