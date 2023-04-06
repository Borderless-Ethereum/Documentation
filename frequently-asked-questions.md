# ❔ Frequently Asked Questions

## Why not just use existing data on the geographical distribution of nodes?

The existing data that is available tracks the geographical distribution of ALL nodes on the network. However, only a subset of these nodes are actually validator nodes, and these are the ones that we are interested in finding the geographical distribution of. Validator nodes are the ones that actually propose blocks to the network and collect attestations from other validator nodes, and so are a critical component of Ethereum's infrastructure.

## What do I have to do to participate?

That's the easy part, just configure the consensus client of your node to put a "geo-tag" in the graffiti field of the blocks you propose. More information on the geo-tag and how to configure specific clients can be found here.

## Will this compromise my security as a validator node?

Not at all! We only want to find out what country your node is situated in, and not the exact location. Your IP address and other details will remain private, and the only that is shared is what you place in the graffiti field of the blocks you publish!

## When will the results be available?

The results will be made available over the next couple of months on this website and we'll update everyone as soon as we have an update.

## What do you plan to do with this data?

This data will help the community to understand where nodes are overly concentrated and which parts of the world are under-represented in the network, which will allow us to form proposals for promoting the operation of validator node in those under-represented regions. As we try to encourage the wider distribution of the network's validator set across multiple jurisdictions, we will use this data to measure the efficacy of those efforts on an on-going basis.

## Why not just get this information from mev-boost relayers?

While it might be possible to reverse geo-code a validator's IP address when they connect to a relayer, relayers operators are very hesitant to put in place any infrastructure that process IP addresses at all, for obvious reasons.  It is paramount that the IP address and location of validator nodes remains private.

## Wen Token?

To acknowledge the efforts of validator node operators that decide to participate, we will be dropping an exclusive POAP to the validators who share geo-tags.  When exactly this will happen is still TBD.
