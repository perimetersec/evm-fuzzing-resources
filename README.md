# EVM Fuzzing Resources
This repository provides a collection of resources on EVM fuzzing. It is actively maintained by [Rappie](https://x.com/rappie_eth) and regularly updated for relevance. Check out the [Recent Additions](recent.md) for the latest updates.

If you have suggestions regarding the content, feel free to reach out on X or open a GitHub issue.

## Table of Contents
1. [Fuzzing Software](#fuzzing-software)
2. [Tooling](#tooling)
3. [Practical Code Samples](#practical-code-samples)
4. [Reusable Properties](#reusable-properties)
5. [Articles](#articles)
6. [Videos](#videos)
7. [Fuzzing Background](#fuzzing-background)

## Fuzzing Software

### Mainstream Fuzzers
- [Echidna](https://github.com/crytic/echidna) by [Trail of Bits](https://x.com/trailofbits)
- [Medusa](https://github.com/crytic/medusa) by [Trail of Bits](https://x.com/trailofbits)
- [Foundry](https://github.com/foundry-rs/foundry) by [Paradigm](https://x.com/paradigm)

### Emerging/Specialized Fuzzers
- [ItyFuzz](https://github.com/fuzzland/ityfuzz) by [fuzzland](https://x.com/fuzzland_)
- [Wake](https://github.com/Ackee-Blockchain/wake) by [Ackee](https://x.com/AckeeBlockchain)

## Tooling
### Libraries & Frameworks
- [Chimera](https://github.com/Recon-Fuzz/chimera) - Smart Contract Property-Based Testing Framework, by [Recon](https://x.com/getreconxyz)
- [Fuzzlib](https://github.com/perimetersec/fuzzlib) - Solidity Fuzzing Library, by [Perimeter](https://x.com/perimeter_sec)
- [CallTestAndUndo](https://github.com/Recon-Fuzz/call-test-undo) - Simple abstract contract to help write invariant tests that do not influence the story, by [Recon](https://x.com/getreconxyz)

### Utils
- [fuzz-utils](https://github.com/crytic/fuzz-utils) - Set of Python tools to improve the developer experience when using smart contract fuzzing, by [Trail of Bits](https://x.com/trailofbits)
- [CloudExec](https://github.com/crytic/cloudexec) - A general purpose foundation for cloud-based fuzzing, by [Trail of Bits](https://x.com/trailofbits)
- [echidna-trace-parser](https://github.com/Enigma-Dark/echidna-trace-parser) - A parser that converts echidna call traces into foundry PoC tests, by [Enigma Dark](https://x.com/EnigmadarkLabs)
- [Echidna Coverage Reporter](https://github.com/Simon-Busch/echidna-coverage) - A TypeScript tool to parse and analyze Echidna code coverage reports for Solidity smart contracts, by [0xsi](https://x.com/_0xsi)
- [Echidna Logs Scraper](https://getrecon.xyz/tools/echidna) - Scrape echidna logs for broken properties repros, by [Recon](https://x.com/getreconxyz)

## Practical Code Samples
- [List of Public Fuzzing Campaigns](https://github.com/perimetersec/public-fuzzing-campaigns-list) by [Rappie](https://x.com/rappie_eth)
- [Property-based testing benchmark](https://github.com/aviggiano/property-based-testing-benchmark) by [Antonio Viggiano](https://x.com/agfviggiano)
- [Solidity Fuzzing Challenge: Foundry vs Echidna vs Medusa (plus Halmos & Certora)](https://github.com/devdacian/solidity-fuzzing-comparison) by [Dacian](https://x.com/DevDacian)
- [Fuzzer Gas Metric Benchmark](https://github.com/rappie/fuzzer-gas-metric-benchmark) by [Rappie](https://x.com/rappie_eth)
- [Reproduction of the $41M Curve reentrancy hacks on July 30 2023 using on-chain fuzzing with Echidna](https://github.com/rappie/echidna-curve-reentrancy-hack) by [Rappie](https://x.com/rappie_eth)
- [Reproduction of the $80M Rari Finance Hack on April 30 2022 using on-chain fuzzing with Echidna](https://github.com/rappie/echidna-rari-hack) by [Rappie](https://x.com/rappie_eth)

## Reusable properties
- [ERC20](https://github.com/crytic/properties?tab=readme-ov-file#erc20-tests) by [Trail of Bits](https://x.com/trailofbits)
- [ERC721](https://github.com/crytic/properties?tab=readme-ov-file#erc721-tests) by [Trail of Bits](https://x.com/trailofbits)
- [ERC4626](https://github.com/crytic/properties?tab=readme-ov-file#erc4626-tests) by [Trail of Bits](https://x.com/trailofbits)
- [ABDKMath64x64](https://github.com/crytic/properties?tab=readme-ov-file#abdkmath64x64-tests) by [Trail of Bits](https://x.com/trailofbits)
- [ERC7540](https://github.com/Recon-Fuzz/erc7540-reusable-properties) by [Recon](https://x.com/getreconxyz)

## Articles
### Tutorials & Guides
- [Echidna Tutorial](https://github.com/crytic/building-secure-contracts/tree/master/program-analysis/echidna) by [Trail of Bits](https://x.com/trailofbits)
- [Medusa Official Documentation](https://secure-contracts.com/program-analysis/medusa/docs/src/index.html) by [Trail of Bits](https://x.com/trailofbits)
- [Foundry Invariant Testing Official Documentation](https://book.getfoundry.sh/forge/invariant-testing)
- [Invariant Testing WETH With Foundry](https://mirror.xyz/horsefacts.eth/Jex2YVaO65dda6zEyfM_-DXlXhOWCAoSpOx5PLocYgw) by [horsefacts](https://x.com/eth_call)
- [Introduction to fuzzing](https://allthingsfuzzy.substack.com/p/introduction-to-fuzzing) by [bloqarl](https://x.com/TheBlockChainer)
- [Benefits of Fuzzing](https://github.com/perimetersec/resources/blob/main/services/Benefits%20of%20Fuzzing.md) by [Perimeter](https://x.com/perimeter_sec)
- [Creating Invariant Tests for an AMM Smart Contract](https://allthingsfuzzy.substack.com/p/creating-invariant-tests-for-an-amm) by [bloqarl](https://x.com/TheBlockChainer)
- [Debugging Echidna Coverage](https://allthingsfuzzy.substack.com/p/debugging-echidna-coverage) by [nican0r](https://x.com/nican0r) 
- [First Day At Invariant School](https://getrecon.substack.com/p/first-day-at-invariant-school) by [nican0r](https://x.com/nican0r) 
- [Generating unit tests from broken stateful invariant tests](https://allthingsfuzzy.substack.com/p/generating-unit-tests-from-broken) by [nican0r](https://x.com/nican0r) & [Antonio Viggiano](https://x.com/agfviggiano)
- [Finding Denial of Service Bugs At Scale With Invariant Tests](https://allthingsfuzzy.substack.com/p/finding-denial-of-service-bugs-at) by [Antonio Viggiano](https://x.com/agfviggiano)
- [Using Echidna to test a smart contract library](https://blog.trailofbits.com/2020/08/17/using-echidna-to-test-a-smart-contract-library/) by [Trail of Bits](https://x.com/trailofbits)
- [Building A Test Harness With Recon](https://getrecon.substack.com/p/building-a-test-harness-with-recon) by [nican0r](https://x.com/nican0r)
- [How To Define Invariants](https://getrecon.substack.com/p/how-to-define-invariants) by [nican0r](https://x.com/nican0r)
- [Implementing Your First Smart Contract Invariants: A Practical Guide](https://getrecon.substack.com/p/implementing-your-first-few-invariants) by [nican0r](https://x.com/nican0r)
- [10 Steps To Easily Use 3 Fuzzers](https://x.com/DevDacian/status/1733009929508917499) by [Dacian](https://x.com/DevDacian)

### Research & Background
- [Learnings from 6 weeks of fuzzing Badger DAO's eBTC protocol](https://allthingsfuzzy.substack.com/p/learnings-from-6-weeks-of-fuzzing) by [Antonio Viggiano](https://x.com/agfviggiano)
- [A Guide to Crafting Robust Invariants](https://allthingsfuzzy.substack.com/p/a-guide-to-crafting-robust-invariants) by [Web3Sec News](https://substack.com/@web3secnews) & [Antonio Viggiano](https://x.com/agfviggiano)
- [Certora vs Echidna: a case study on invariant testing in eBTC](https://allthingsfuzzy.substack.com/p/certora-vs-echidna-a-case-study-on) by [nican0r](https://x.com/nican0r)
- [Uniswap v3: A Fuzzing Review](https://allthingsfuzzy.substack.com/p/uniswap-v3-a-fuzzing-review) by [nican0r](https://x.com/nican0r)
- Lessons Learned From Fuzzing Centrifuge Protocol [part 1](https://getrecon.substack.com/p/lessons-learned-from-fuzzing-centrifuge) & [part 2](https://getrecon.substack.com/p/lessons-learned-from-fuzzing-centrifuge-059) by [nican0r](https://x.com/nican0r)
- [eBTC Retrospective: A reflection on lessons learned in our extended fuzzing of eBTC](https://getrecon.substack.com/p/ebtc-retrospective) by [nican0r](https://x.com/nican0r) 
- [Lessons From The Fuzzing Trenches](https://getrecon.substack.com/p/lessons-from-the-fuzzing-trenches) by [nican0r](https://x.com/nican0r) 
- [Finding Real Vulnerabilities with the Renzo Fuzzing Repo](https://getrecon.substack.com/p/finding-real-vulnerabilities-with) by [nican0r](https://x.com/nican0r) 
- [Fuzzing in the Cloud: A review of the different cloud based options for fuzzing Solidity contracts](https://getrecon.substack.com/p/fuzzing-in-the-cloud) by [nican0r](https://x.com/nican0r) 
- [Corn Engagement Retrospective: Lessons learned from our engagement fuzzing the Corn protocol](https://getrecon.substack.com/p/corn-engagement-retrospective) by [nican0r](https://x.com/nican0r) 

## Videos
### Tutorials & Guides
- [Learn how to fuzz like a pro](https://www.youtube.com/playlist?list=PLciHOL_J7Iwqdja9UH4ZzE8dP1IxtsBXI) - Fuzzing workshop, by [Trail of Bits](https://x.com/trailofbits)
- Introduction to Fuzzing, Foundry, Echidna & Medusa, by [bloqarl](https://x.com/TheBlockChainer)
	- [part 1](https://www.youtube.com/watch?v=xLGTd5OH8xU), [part 2](https://www.youtube.com/watch?v=dWyJq8KGATg), [part 3](https://www.youtube.com/watch?v=yUC3qzZlCkY), [part 4](https://www.youtube.com/watch?v=em8xXB9RHi4), [part 5](https://www.youtube.com/watch?v=I4MP-KXJE54), [part 6](https://www.youtube.com/watch?v=SSzh5GlqteI)
- [Invariant Testing WETH with Foundry](https://www.youtube.com/watch?v=sJpL21yJpgs) by [horsefacts](https://x.com/eth_call)
- [Invariant Driven Development - Build a CDP system using Invariants as Safety Nets](https://youtu.be/ZM6479HeI5U?si=7Zlbq8Ao4y1sFtSw) by [Alex the Entreprenerd](https://x.com/GalloDaSballo)

### Talks & Discussion
- [Web3 Security: All Things Fuzzing with Victor Martinez](https://www.youtube.com/watch?v=83q14K-WNKM) by [vnmrtz.eth](https://x.com/vn_martinez_)
- [Fuzzing and Heuristics interview with @devdacian](https://www.youtube.com/watch?v=IZTvXfC14Ig), by [Cyfrin Audits](https://x.com/CyfrinAudits) 
- [Fuzzing Like a Degen: Building a Smart Contract Fuzzer](https://youtu.be/qdtQ9k3gCX8?si=AquZxyikCZJwRaU5) by [alpharush](https://x.com/0xalpharush)
- [All Things Fuzzing with Victor Martinez](https://youtu.be/83q14K-WNKM?si=ez3uZRBvm-3iksFT) by [vnmrtz.eth](https://x.com/vn_martinez_)
- [Advanced Fuzzing Techniques: An eBTC Case Study](https://youtu.be/ELY_zjIAKuE?si=1CfWOLuRaeTwQVT2) by [Antonio Viggiano](https://x.com/agfviggiano)
- [Invariant Testing Workshop](https://youtu.be/YAF79t_Sfiw?si=AhJ-0pepG6-P_Ux8) by [Antonio Viggiano](https://x.com/agfviggiano)
- [Euler v2 Fuzzing Workshop by Víctor Martinez](https://youtu.be/WO3Xu7E4Tdg?si=MuQ1LJERLjRc8Pdc) by [vnmrtz.eth](https://x.com/vn_martinez_)
- [Size Credit Fuzzing Workshop](https://youtu.be/tShSMDVoBf8?si=wztKs7dO7mCWfiXq) by [Antonio Viggiano](https://x.com/agfviggiano)
- [Test your tests The dos and don'ts of testing](https://www.youtube.com/watch?v=7TcnUZGuk_s) by [phaze](https://x.com/lovethewired)
- [Find Highs Using Invariant Fuzz Testing](https://www.youtube.com/watch?v=Cqmu-mhSLt8&t=15s) by [Dacian](https://x.com/DevDacian)
- [Submit your first PR to Medusa](https://www.youtube.com/watch?v=Cqmu-mhSLt8&t=3855s) by [Josselin Feist](https://x.com/Montyly)
- [A glimpse into the future of invariant testing](https://www.youtube.com/watch?v=Cqmu-mhSLt8&t=5627s) by [Alex the Entreprenerd](https://x.com/GalloDaSballo)
- [You should probably be fuzzing](https://www.youtube.com/watch?v=Cqmu-mhSLt8&t=6565s) by [Daniel Von Fange](https://x.com/danielvf)
- [Echidna Made Me Do It!](https://www.youtube.com/watch?v=Cqmu-mhSLt8&t=8030s) by [Alex the Entreprenerd](https://x.com/GalloDaSballo)
- [Uniswap V4: Taking Invariant Testing Where Manual Review Cannot Go](https://www.youtube.com/watch?v=Cqmu-mhSLt8&t=8991s) by [Benjamin Samuels](https://x.com/thebensams)

## Fuzzing Background
- [The Fuzzing Book](https://www.fuzzingbook.org/) - Tools and Techniques for Generating Software Tests, by [Multiple Authors](https://x.com/FuzzingBook)
- [Awesome Fuzzing](https://github.com/secfigo/Awesome-Fuzzing) - A curated list of fuzzing resources for learning Fuzzing, by [Mohammed A. Imran](https://x.com/secfigo)
