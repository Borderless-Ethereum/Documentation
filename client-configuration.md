---
description: How to configure your respective client software to participate
---

# ⚙ Client Configuration

## Client Configurations

### Prysm <a href="#prysm" id="prysm"></a>

**Documentation:** [https://docs.prylabs.network/docs/prysm-usage/graffiti-file](https://docs.prylabs.network/docs/prysm-usage/graffiti-file)

The --graffiti-file flag for the Prysm validator client allows you to add graffiti to blocks. Different graffiti may be configured for different validators running in the same process.

**Usage:**

```
--graffiti-file=/path/to/graffitis.yaml
```

**Example:**

```
specific:
  163: "validator 163 was here"
  914: "validator 914 was here"
  546: "validator 536 was here"
  237: "validator 237 was here"
random:
  - "Mr A was here"
  - "Mr B was here"
  - "Mr C was here"
default: "Mr F was here"
```

### Lighthouse <a href="#lighthouse" id="lighthouse"></a>

**Documentation:** [https://lighthouse-book.sigmaprime.io/graffiti.html](https://lighthouse-book.sigmaprime.io/graffiti.html)

**Usage:**

```
lighthouse vc --graffiti-file graffiti_file.txt
```

**Example:**

```
default: default_graffiti
public_key1: graffiti1
public_key2: graffiti2
```

### Teku <a href="#teku" id="teku"></a>

**Documentation:** [https://docs.teku.consensys.net/Reference/CLI/Subcommands/Validator-Client#validators-graffiti](https://docs.teku.consensys.net/Reference/CLI/Subcommands/Validator-Client#validators-graffiti)

**Usage:**

```
teku vc --validators-graffiti-file=<FILE>
```

> File containing the validator graffiti to add when creating a block. The file content is converted to bytes and padded to Bytes32. The same graffiti is used for all validators started with this beacon node.

### Nimbus <a href="#nimbus" id="nimbus"></a>

**Documentation:** [https://nimbus.guide/graffiti.html](https://nimbus.guide/graffiti.html)

You can use your node’s graffiti flag to include a short text in the blocks that your node creates. You will be able to see it using the block explorer.

**Usage:**

```
./run-mainnet-beacon-node.sh --graffiti="<YOUR_WORDS>"
```

***

### Lodestar <a href="#lodestar" id="lodestar"></a>

**Documentation:** [https://chainsafe.github.io/lodestar/reference/cli/#validator](https://chainsafe.github.io/lodestar/reference/cli/#validator)

Specify your custom graffiti to be included in blocks (plain UTF8 text, 32 characters max)

**Usage:**

```
validator --network goerli --graffiti "Your Graffiti"	
```
