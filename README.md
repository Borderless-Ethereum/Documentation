# 🚀 About this Project

## Our Vision

{% hint style="info" %}
We're trying to measure the geographical distribution of validator nodes as a measure of how vulnerable or resilient Ethereum is to nation state coercion. We're calling all validator node operators to help us!
{% endhint %}

For Ethereum to be a credibly neutral platform that remains resistant to coercion from nation states, it must maintain a healthy geographical and jurisdictional distribution of validator nodes.

In order to encourage geographical distribution of validators, we first need to be able to measure it, and we need to do this in a way that protects validator privacy for security reasons, i.e. we only need to know which country validators are based in.

To achieve this goal we are asking validator nodes to self-report their country of operation by including a small tag in the graffiti field of the blocks they propose.

## Here's how it works

* As a node operator, configure your client to put a geo-code in the graffitti field of the blocks you produce
* The geo-code should look like "GEO-XX" where XX is the country code of the country your node is situated in
* We will scan the beacon chain for geo-codes and compile a database of how many nodes are in which country
