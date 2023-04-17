# ❔ Frequently Asked Questions

## Why not just use existing data on the geographical distribution of nodes?

The existing data that is available tracks the geographical distribution of ALL nodes on the network. However, only a subset of these nodes are actually validator nodes, and these are the ones that we are interested in finding the geographical distribution of. Validator nodes are the ones that actually propose blocks to the network and collect attestations from other validator nodes, and so are a critical component of Ethereum's infrastructure.

## What do I have to do to participate?

That's the easy part, just configure the consensus client of your node to put a "geo tag" in the graffiti field of the blocks you propose. More information on the geo tags and how to configure specific clients can be found [here](list-of-country-codes.md).

## Will this compromise my security as a validator node?

Not at all! We only want to find out what country your node is situated in, and not the exact location. Your IP address and other details will remain private, and the only information that is shared is what you place in the graffiti field of the blocks you publish!

## When will the results be available?

The results will be made available over the next couple of months on this website and we'll update everyone as soon as we have an update.

## What do you plan to do with this data?

This data will help the community to understand where nodes are overly concentrated and which parts of the world are under-represented in the network, which will allow us to form proposals for promoting the operation of validator nodes in those under-represented regions. As we try to encourage the wider distribution of the network's validator set across multiple jurisdictions, we will use this data to measure the efficacy of those efforts on an on-going basis.

## What if I have separate Validator Client and Beacon Node and they are not co-located?

We are only interested in which country the Validator Client is situated in, so that's the country that you specify in the geo tag, not the beacon node. In the case that multiple Validators Clients are connected to a single Beacon Node and those validators are all in different countries, then place a geo tag for each country in the graffiti field.

## Why not just get this information from mev-boost relayers?

While it might be possible to reverse geo-code a validator's IP address when they connect to a relayer, relayer operators are very hesitant to put in place any infrastructure that processes IP addresses at all, for obvious reasons. It is paramount that the IP addresses and locations of validator nodes remains private.

If I put a geo tag in my graffiti, can I still put other things in their too?

Yes! You can place the geo tag at the start, middle or end of the graffiti field, mixed in with other content, and we'll still pick it up!

## Wen Token?

To acknowledge the efforts of validator node operators that decide to participate, we will be dropping an exclusive POAP to the validators who share geo tags.  When exactly this will happen is still TBD.

## What if my fee recipient is a staking pool, how do I get a POAP?

Obviously by using the fee recipient of the execution block, we can't drop POAPs to the node operators of staking pool's validators, because the fee recipient points to a shared pool. We're currently working with staking pools to determine how participating node operators can claim a POAP.
