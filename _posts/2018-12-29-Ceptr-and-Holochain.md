---
layout: post
title: Ceptr and Holochain - Currencies of Social Coherence. Holography and Distributed Hash Tables vs. Consensus Bottlenecks in Monolithic Blockchain Ledgers.
---

![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1e/Pieter_Bruegel_the_Elder_-_Children%E2%80%99s_Games_-_Google_Art_Project.jpg/1024px-Pieter_Bruegel_the_Elder_-_Children%E2%80%99s_Games_-_Google_Art_Project.jpg)

> *"Perhaps the first thing that comes to mind when thinking about science fiction and money is the different kinds of currencies that are imagined for future worlds: the poscreds of Philip K. Dick’s Ubik, a currency required for every minute transaction such that the door becomes not an item you own but, rather, a provider of services for which you must continually pay, leaving protagonist Joe Chip trapped in his own apartment until someone pays his door to open; the bars of gold-pressed latinum used by the avaricious Ferengi on Star Trek, the only thing that cannot be replicated in this post-scarcity world, useless other than as an atavistic marker of wealth; the reputation- based currency of whuffie in Cory Doctorow’s Down and Out in the Magic Kingdom, used to replace the social role money plays in creating a hierarchy in another post-scarcity world.* 
>
> ***The inventiveness of SF writers creating objects or systems of account that might serve as money is matched by its actual history and the wide range of items that have served as currency, from large stone wheels called Rai used as money on the island of Yap, to the split tally sticks of medieval English practice, to coinage and the ideal that a gold standard is the ‘real’ value of money, to slips of paper inscribed with various authentications and, finally, to the electronic signals used to store and transmit denominations of value.*** 
>
> ***It turns out that, although most of the world uses money on a daily basis and has done so for almost as long as there have been records of human civilization, it is not very clear what money actually is. How does money work? What is the underlying relationship among some underlying thing of ‘actual’ value (gold, land, the goods and services produced by a nation), the tokens of that value (coins, banknotes, electronic account balances) and the entity guaranteeing that said tokens are, basically, the same as that underlying thing of value (the King, the Bitcoin algorithm, the European Union). Reading about the history of money turns out to be surprisingly like reading science fiction: the kind of money a society has tells us a lot about the kind of human sociality that is possible in that world."***
>
> - Sherryl Vint, "Currencies of Social Organization: The Future of Money" 

The above cited passage seems an appropriate starting point for framing [Holochain](https://holochain.org/) - a non-blockchain architecture for distributed social applications (dApps or hApps) and the ground level for further expanding an evolvable, fully distributed framework for coordinated sense-making and collective value-creation (i.e., means of articulating value) on all scales. Even though it had been conceived of and slowly developed for over more than a decade (by a group of people with already significant experience in designing systems currencies), Holochain only recently came to wider attention with an Initial *Community* Offering, [Holo](https://holo.host) - a set of base application components and modules intended to introduce Holochain to the wider public and set the wheels in motion (the hApp prototying and development tools are designed to make development as straightforward, accessible and easy to understand as possible, somewhat similar to a simple web development framework).

Instead of extending, modifying and reiterating upon the usual monolithic blockchain base, Holochain brings in a wholly different architecture for decentralized data coordination based on [distributed hash tables](https://en.wikipedia.org/wiki/Distributed_hash_table) (DHTs) as the public space (a familiar implementation of which is the BitTorrent file sharing mechanism). DHTs are tables of key-value pairs stored in overlapping shards among network peers. They provide a highly efficient and generalizable basis for managing application data and carrying out routing across large-scale peer-to-peer networks. Agents, by virtue of their agency, can easily bridge between the spaces of different Holochain applications (hApps), translating one context into another or importing validated datasets from one app into another. Holochain is, as such, an agent-centric model, whereas blockchains and most other forms of DLT are data-centric, rigidly deterministic and highly limited in their functional capacities (Bitcoin is said to have engineered artificial scarcity supported by an arms race lottery of enormous waste, so-called "proof-of-work"). 

This general arrangement sets the stage for a quickly expanding pool of diverse hApps and their rich networks of flowing information, available for agents/users to pull into all kinds of possible compositional abstractions, combining different flow indicators (as hApps or reusable functional components) in information system feedbacks. Additionally, it is extremely lightweight and highly scalable (DHTs are *already* pragmatically sharded between the relevant participants) - a set of properties that immediately resolve all the critical flaws of blockchain-based systems (scalability, sustainability and social consensus). 

![](https://i.imgur.com/O3Ksy8b.jpg)

*Distributed Hash Tables store key-value pairs where any node can retrieve the value associated with a given key as a lookup service. Maintaining the key-to-value mappings is distributed among peering nodes.*

Such sharded agent-centric model alleviates the burden of having to (similar to lie-detector [polygraphs](https://en.wikipedia.org/wiki/Polygraph)) replicate the same output across all nodes in the network, forming agency around individual actors and the kinds of relationships they enter into instead (each agent storing only what is relevant to him). Agents record and store data in their individual source chains (or [hashchains](https://en.wikipedia.org/wiki/Hash_chain)), unfolding parts of them onto the respective app DHTs (private and public space, respectively) and mutually audited (according to the implied validation rules) and countersigned records of transactions with other agents in their source chains.

As mentioned, there is no notion of network-wide consensus (which, by definition, doesn't scale) bottlenecking the system and strictly limiting the kinds of flows that can enter and the ways in which it can be seen and translated between different contextual interpretations as useful information (and from the reference point of a given agent's view of the network, or in other words, data is understood as relative to the circumstances at hand, not as an absolute, objective category). DHTs as such constitute a form of *sharded validation* (what Ethereum is looking to eventually accomplish with PoS+sharding, now known as Ethereum 2.0) where participants store only those shards they happen to validate.

> # currency (n.)
>
> 1650s, "condition of flowing," a sense now rare or obsolete, from Latin *currens*, present participle of *currere* "to run". The notion of "state or fact of flowing from person to person" led to the senses "continuity in public knowledge" (1722) and "that which is current as a medium of exchange, money" (1729).

Important to keep in mind is that Holochain is just one of the functional building block components of a broader initiative called [Ceptr](http://ceptr.org) (from *receptor*, as it employs a [bio-inspired, ecosystemic](https://en.wikipedia.org/wiki/Biomimetics) approach to computation and organizing  complexity). Though Holochain is separately introduced on its own first with Holo (ticker [HOT](https://coinmarketcap.com/currencies/holo/)) as its entry into the mainstream. [Holo](https://holo.host) brings the economic ingredient needed for setting things in motion and forming the basis for a gradually expanding ecosystem around distributed holochain applications (hApps).

Presently an [ERC-20](https://en.wikipedia.org/wiki/ERC-20) receipt, HOT is to be redeemed for Holo fuel upon launching in the first quarter of 2019. Holo fuel is a [mutual-credit crypto-currency](http://ceptr.org/whitepapers/mutual-credit) and an accounting system put in place as means for payment and settlement of application hosting imbalances. Developers will initially be paying host providers in Holo fuel to host their applications and provide their service to other users (via [Holoport devices](https://medium.com/h-o-l-o/holoport-manufacturing-has-begun-25935796af76) specifically designed for the purpose, or as configured on any other regular device) without their own running instances of a Holochain node (that way making hApps accessible from any web browser). Some of the applications supported within the Holo app ecosystem will include:

- Distributed PKI (Public Key Infrastructure)
- Distributed Directories
- Rating/Tagging/Annotation
- Chat & Social posting
- Distributed Content Delivery Network
- A crypto-reputation-currency akin to a BitTorrent sharing ratio

The scope of Ceptr however stretches much farther than that, envisioned as gradually colonizing and extending into a globally entangled nervous system, a "quantum leap in large-scale collective social intelligence" (as [reflected in notions such as](http://ceptr.org/whitepapers/) *distributed associative memory* and *large-scale self-reflective functional intelligence* in some of the initially drafted papers) where flows of information can be pulled and arranged in composite abstractions of meaning and distributed sense-making at scale. As one of the project paper drafts, ["Grammatic Capacities and the Evolution of Complex Adaptive Systems"](http://ceptr.org/whitepapers/grammatics) explains: 

>  The fundamental insight comes from the observation that **new complex adaptive systems, as well as fundamental changes within those systems always appear concomitant with the emergence of a special type of informational infrastructure.** We call such an infrastructure a Grammatic Capacity and propose a formalism to describe them abstractly, as well as offer a proof-of-concept new Grammatic Capacity for catalyzing change in the complex adaptive system we call human society.

And further in the [published project outlines](http://ceptr.org/projects/neural):

> The generalized ability to plant persistent listeners for specific state changes in other’s applications, **enables the weaving of synaptic like connections across a whole network. These patterns are exactly the kinds of synaptic patterns of learning neural networks.**
>
> **In the case of Ceptr, humans may be doing the learning and consciously trying out new connections. Or machines and algorithms could be tuning connections and patterns. Either way, this feature combined with the fundamental interoperability of self-describing protocols makes for exciting prospects of true Synthetic Intelligence – not Artificial Intelligence separate from people, but scaling collective intelligence with humans integrated in the heart of it in healthy distributed ways.**

If the purpose of blockchained ledgers had been to serve as a kind of institutional technology of "code is law" baked into the level of the network protocol itself, then Ceptr's purpose is to instead provide the means for actively making sense (from immutable and tamper-proof data, filtered through the respective app validation rules) and revealing productive flows and correlations in the socio-technical fabric we occupy (and in which are often subtly tricked and manipulated by those that happen to control the medium of technology) - since, we shouldn't forget, the only valid model of a human system is the system itself, thus it should necessarily allow for enough room and flexibility for the system to organically model itself (whereas blockchains are enclosed, walled off systems that operate in a linear, deterministic fashion).

> *Blockchain is about managing a consensus about what was “said.” Ceptr is about distributing a consensus about how to “speak.”*
>
> - Arthur Brock, Holo Co-Founder and Acting CEO

One example of the kind of reasoning and approach Ceptr applies to exploring how meaning is organically constituted from various diverse units and elements across dimensions and scales [would be a recent publication from the Max Planck Institute for Psycholinguistics](http://maxplanck.nautil.us/article/341/brainwaves-encode-the-grammar-of-human-language) about how brainwaves encode grammar:

> They [Scientists at the University of Edinburgh and the Max Planck Institute] constructed an artificial neural network that simulates key features of the brain, such as densely connected populations of neurons that show neural oscillations. Neural oscillations are wave-like patterns of activity that happen at different frequencies, some very fast and some slow. The relative timing of these neural oscillations can help the brain encode grammatical relationships between words in a sentence, as Andrea Martin and Leonidas Doumas report in a paper in *PLOS Biology*.
>
> [...]
>
> **Linking our brains to our behaviors holds the key to understanding not only what it means to be human, but also to understanding how the (arguably) most complex computing device in the universe, the human brain, gives rise to our daily experiences. Such knowledge may also lead to biologically inspired advances in human-like artificial intelligence and computation.**

The overall rationale is also echoed in French philosopher [Gilles Deleuze's](https://en.wikipedia.org/wiki/Gilles_Deleuze) (of whom Foucault famously said that "the 21th century will be Deleuzian") conception of the [rhizome](https://en.wikipedia.org/wiki/Rhizome_(philosophy) ) as the *image of thought* coming to define the character of our emerging new era: 

>  **"A multiplicity has neither subject nor object, only determinations, magnitudes, and dimensions that cannot increase in number without the multiplicity changing in nature (the laws of combination therefore increase in number as the multiplicity grows). Puppet strings, as a rhizome or multiplicity, are tied not to the supposed will of an artist or puppeteer but to a multiplicity of nerve fibers, which form another puppet in other dimensions connected to the first: "Call the strings or rods that move the puppet the weave. It might be objected that its multiplicity resides in the person of the actor, who projects it into the text. Granted; but the actor's nerve fibers in turn form a weave. And they fall through the gray matter, the grid, into the undifferentiated... The interplay approximates the pure activity of weavers attributed in myth to the Fates or Norns."** An assemblage is precisely this increase in the dimensions of a multiplicity that necessarily changes in nature as it expands its connections. There are no points or positions in a rhizome, such as those found in a structure, tree, or root. There are only lines. When Glenn Gould speeds up the performance of a piece, he is not just displaying virtuosity, he is transforming the musical points into lines, he is making the whole piece proliferate."
>
> - Gilles Deleuze & Felix Guattari, *"A Thousand Plateaus"*

The above beautifully illustrates the notion of how events, concepts, rhythms and cycles, etc. express themselves as they traverse through different dimensions, domains and bodies (referred to as "multiplicity", which fundamentally asserts that there is more than one geo-historical trajectory). In an important way, Ceptr aims to provide the means for developing and incorporating many such different *expressive capacities* (alphabetic language and money being just two relatively limited such capacities), which in turn reveal and allow for weaving the appropriate, adequate terms necessary for framing a problem so that the range of possible (valid) solutions naturally becomes self-evident from the formulation of the problem as such (a general property of mathematics as language, but also art). 

Since [ontology](https://en.wikipedia.org/wiki/Ontology) (the categories of being, or what *is* and how it can be related, e.g. subject-predicate sentence constructions) conditions [epistemology](https://en.wikipedia.org/wiki/Epistemology) (what can be *known* about what *is*) and since we tend to be limited in what we can see by what we already know, Ceptr's ambitious (and in all likelihood extremely important for our sustainable future as complex technological societies) role is to expand the ontological reach of *what* can be related and *how* (i.e., multi-disciplinary approaches that integrate diverse views and methods), revealing in the process the often hidden inter-dependencies and dynamic relations that constitute the entangled web of non-linear complex systems around us (such as, for example, the global economy, the nervous system and its technological prosthetic extensions as global communications and the Internet, etc.) - the conceiving of currencies as **"current-sees"** reflecting of that understanding.

![](https://i0.wp.com/metacurrency.org/wp-content/uploads/2016/08/Currency_System_Life_Cycle.png?fit=1142%2C1677)

Currencies/current-sees in Ceptr are not limited to monetary and/or capital flows, but can be said to be anything around which individual elements organize as a coherent larger whole (as for example classrooms and schools, villages and cities, nation-states, etc.) Reputation, for example, can be said to be a non-exchangeable currency. So, Ceptr also can be considered as providing a general framework for designing currencies as such, in the cyberspace domain of how we sometimes organize as communities and have gotten accustomed to how communication technologies shorten time and space between us. 

As the underlying data integrity engine of Ceptr, Holochain first lays the foundations to build upon and has drawn significant interest from, among others, the Ethereum developer community and Mozilla (as well as having become 4chan's new focus of attention and constant hype, pushing ChainLink aside). Below, we'll explore some of the technical specifications and practical details surrounding Holochain and the upcoming Holo launch.

## Structure and Functionality of an hApp

hApps are essentially scripts hooked to distributed databases. The basic logic and backbone of an hApp is defined in its DNA file (usually a [Javascript Object Notion](https://en.wikipedia.org/wiki/JSON), or JSON file). [Zomes](https://holochain.github.io/rust-api/0.0.1/hdk/macro.define_zome.html) are modular components defining the functionalities integrated (and usually take one argument - either as string or a JSON object). Zome functions are exposed to the UI and mediate agent actions received through the DNA and recorded as chain entries. Chain entries can be either publicly shared (into the DHT) or privately committed. 

Transacting/interacting agents audit each other's chains according to the implied validation rules and counter-sign each other's entries. Their peers further validate the transactions, extending into a complex history of associations and transactions that resembles a massive [DAG](https://en.wikipedia.org/wiki/Directed_acyclic_graph) (directed acyclic graph) or, to again try and be [Deleuzian](https://en.wikipedia.org/wiki/Gilles_Deleuze) about it, a [rhizome](https://en.wikipedia.org/wiki/Rhizome_(philosophy) ). The hApp's DHT holds the DNA backbone, the agents' public keys, the chain entry headers and all associated publicly committed data, as well as links between address points (app-specific validation rules can put constraints on who is allowed to link to what in an agent's hApp) and warrants as evidence against bad actors (misbehavior is immediately visible and actions taken accordingly).

![](http://ceptr.org/images/Holochain_Subsystems.png)

*Holochain sub-system components: a publicly shared DHT with application functions (zomes) translating and mediating back and forth between individual agent source chains and app-specific DHTs.*

In the world of decentralization, DHTs have really had a revolutionary effect - the chaotic, ad hoc topologies of the first-gen P2P architectures have evolved into a set of topologies with emergent order, provable properties and superb performance. Research DHTs (such as [Kademlia](https://en.wikipedia.org/wiki/Kademlia), Chord, etc.) are starting points for developing custom schemes, each having properties that can be flexibly combined in a multitude of ways. Storage and lookups in DHTs are distributed among multiple machines and all nodes are peers that can freely join and leave the network. Despite the apparent chaos of arbitrary periodic changes to the membership of the network, DHTs make provable guarantees about performance.

hApp DHTs are of the [Kademlia](https://en.wikipedia.org/wiki/Kademlia) type, which uses a [XOR-based](https://en.wikipedia.org/wiki/Exclusive_or) metric for locating nodes and routing queries (i.e, calculating distances in address space between nodes/peers). It has the property of conveying/reinforcing useful contact information along with every message passed between peers, thereby strengthening fault-tolerance and consistency.

### Current Rust Implementation of the Holochain Client

Recently, a [Rust rewrite](https://github.com/holochain/app-spec-rust/releases/tag/v0.0.1-dev-preview) of the initial Go-based Holochain prototype was released. One main reason for making such move is to do with being adaptable to [WebAssembly](https://en.wikipedia.org/wiki/WebAssembly) (WASM) - a critical foundation for a thriving peer-to-peer app ecosystem, ensuring open-ended flexibility that can only improve as WASM grows in popularity and expands support for new languages. A [Rust HDK](https://github.com/holochain/holochain-rust) (Holochain Development Kit) is presently available, with others adapted to [languages compiling to WASM bytecode](https://github.com/appcypher/awesome-wasm-langs) to gradually come about in the near future.

WebAssembly itself first emerged in March 2017 as a web standard defining a binary and assembly-like text format for executable code in Web pages (meant to accelerate execution to nearly as quick as running native machine code). A cross-browser, cross-platform, cross-language initiative originally meant as a complementary to Javascript in speeding up performance-critical parts of web applications, WASM is today being adapted to enable web development in a range of languages other than JavaScript.

Holochain zomes themselves (the parts that define hApp functions) are written in WASM and there is no way that WASM functions can understand the Rust [type system](https://en.wikipedia.org/wiki/Type_system) natively, so sharing any data between holochain core and zome functions must be serialized into JSON strings (which can then be allocated for WASM to read out and deserialized into Rust types/structs/enums). The Holochain-specific Rust HDK macros for defining entities and zomes does most of the memory work and serialization round trips. The ability to serialize [UTF-8](https://en.wikipedia.org/wiki/UTF-8) data and allocate it to memory for communicating it to Holochain core is the main requirement for an HDK based on any (of [the many](https://github.com/appcypher/awesome-wasm-langs), including Python, Lua, Perl and Ruby) languages that compile to WASM.

```bash
$ ./hc
hc 0.0.1
Holochain Core Dev Team <devcore@holochain.org>
A command line for Holochain

USAGE:
    hc <SUBCOMMAND>

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information

SUBCOMMANDS:
    agent       Starts a Holochain node as an agent
    generate    Generates a new zome and scaffolds the given capabilities
    help        Prints this message or the help of the given subcommand(s)
    init        Initializes a new Holochain app at the given directory
    package     Builds the current Holochain app into a .hcpkg file
    test        Runs tests written in the test folder
    unpack      Unpacks a Holochain bundle into it's original file system structure
    web         Starts a web server for the current Holochain app
```

*The `hc` executable packs all the Holochain core functionality.*

The Holochain client initializes hApps and agent nodes, generates zomes and launches web servers that serve hApps (and packages hApps into compact *hcpkg* files). 

A scaffolding tool for easily generating basic DNA files is available [here](https://holochain.github.io/scaffold/). Writing the zomes/functions in Rust is fairly straightforward, the HDK making use of macros (documentation available [here](https://holochain.github.io/rust-api/0.0.1/hdk/macro.define_zome.html)). hApps can be as simple as a basic "Hello world" or as complex as largely distributed social networks like Twitter or Facebook (but without the centralized control, the business model and the involved interests that have resulted in today's highly toxic online environment).

A Medium blog post describing in more detail the step-by-step process of writing/prototyping hApps with the Rust HDK has been made available [here](https://medium.com/holochain/first-steps-writing-holochain-happs-with-rust-80ae111960e). Unlike with Ethereum or other blockchain/DLT frameworks that usually implement their own customized "contract"/scripting language (e.g., Solidity, Vyper, Haskell-based Plutus in Cardano or OCaml-derived Michaelson in Tezos, etc.), Holochain doesn't require that one should learn some new esoteric language and programming paradigm, but allows anybody to use any common programming or scripting language (not just Rust and Javascript).

### Containers

A recent addition, containers are instances containing hApps. A container implements an agent interface, a storage mechanism and a way of communicating with the agent's peers. Instead of shuffling between individual instances and manually managing hApp ports, containers consolidate all communications into a single set of ports within an integrated interface and a shared networking layer - one can have a container for anything, on any platform and/or hApp and have everything involved seamlessly communicate peer-to-peer.

The agent interface, of course, depends on the agent interacting with the Holochain core - a GUI (graphical interface) for an end-user, scriptable and verbose CLI (command-line) for developers running tests, etc. The motivation for the work on containers has been to support the work of the Holo Host team, enabling the needed functionality for making hApps work seamlessly on Holo (think of Holo as a kind of [AWS](https://en.wikipedia.org/wiki/Amazon_Web_Services) for distributed holochain apps, as mentioned earlier).

![](https://i.imgur.com/zyh4z5f.jpg)

*Holo.Host is the edge-hosting platform for the distributed holochain application ecosystem, making them easily accessible through any common web browser. It provides on-demand storage and computing services where "the crowd becomes the cloud."*

![](https://i.imgur.com/1npWL1M.png)

[Holosqape](https://github.com/holochain/holosqape) is a basic GUI container allowing for embedding widgets and buttons for zome functions, along with a Javascript console that hApps can be instantiated in (a proto-holochain browser of sorts). [Websocket](https://github.com/holochain/holosqape#websockets) based connections tie with the hApp front-ends. Some tweaks and adjustments to the networking layer are being made and APIs allowing hApps to modify data (e.g., marking items obsolete instead of deleting, since hashchain and DHT data is itself immutable) added. Regular updates can be found on the [Holochain Design Medium](https://medium.com/@holochain).

## Mutual Credit Accounting and Sovereign Accountable Commons

A mutual credit system of accounting is best suited for some currency applications in a distributed systems economy (Holochain is also a framework for designing social flows as many different kinds of currencies, as already mentioned). Mutual credit accounting is based on the premise that **no unit of currency can be issued out of *fiat*****, but must have an offsetting debit registered in the account-keeping ledger.** Each agent's source chain encodes their balances, so when two parties transact they mutually audit their histories to make sure they have the credits that they're spending. 

Holo comes with the respective accounting infrastructure notarized by the network on the shared DHT, keeping track of Holo fuel via standardized double-entry accounting, which is itself additionally also designed to efficiently handle high-volume micro-transactions and is a value-stable asset, since backed by computational resource, a tangible asset. Holo fuel is just the first example of a Holochain currency implementation - any other design template or configuration can be easily implemented, depending on the desired properties of the currency.

### Sovereign Accountable Commons (SACs) vs. Decentralized Autonomous Organizations (DAOs)

[Sovereign Accountable Commons](http://ceptr.org/projects/sovereign) (SACs) is the Ceptr/Holochain version of what is more commonly known as Decentralized Autonomous Organizations (DAOs) in the blockchain world. SACs run as collectively distributed hApps forming into collectives of equal peers (rather than as a smart contract on a blockchain, the security risks of which are significant as shown with the infamous DAO hack in the early days of Ethereum). Each participant holds copies of their own assets on the SAC-shared DHT, thereby preventing any group or individual into coercing any other else into participating. 

![](http://www.artbrock.com/sites/artbrock.com/files/images/DevAid-HealthyEconomy.png)

Although all data and assets are held in common, they are stored in DHT shards with algorithms adjusting availability and redundancy based on the size and scale of the network. Corruption and sabotage is made instantly visible, allowing that compromised nodes be promptly blacklisted from further access. 

The fractal, localized architecture of such hApps makes them highly scalable without needing to waste resource on energy intensive proof-of-work or making them susceptible to the [Pareto Effect](https://en.wikipedia.org/wiki/Pareto_principle) asymmetries implied in versions of [Proof-of-Stake](https://en.wikipedia.org/wiki/Proof-of-stake) consensus (e.g., the notoriously bad example of EOS' delegated Proof-of-Stake which spells out crypto-plutocracy of openly carried out corruption/coordination by corruption both in theory and practice, so in all likelihood in intention, too).

## Some Further Features of Ceptr

As a semantic framework designed to map out and reify coherent patterns of meaning and organization, an important component of Ceptr is [Semtrex](https://www.codeproject.com/articles/894188/introducing-semtrex) (SEMantic Tree Regular EXpressions) - a universal semantic parser for searching and matching on [semantic trees](http://ceptr.org/blog/2015-04-06-semantic-trees). Semantic trees are the basic data units in Ceptr that receptors (which are lightweight VMs) operate on (instead of, for example, 32 or 64 bit strings) -  the goal being such that meaning/semantics would be built on as low a level of the computing stack as possible so that data carries with it the qualities that give it meaning. Semantic trees are themselves tree-like structures for representing information, where each node in the hierarchy of the tree contains a symbol identifier for the type of data it contains and its respective value. As described in a [blog post](http://ceptr.org/blog/2015-04-06-semantic-trees):

> Semantic trees in Ceptr are like the "Words" of a normal CPU. A regular "word" in a CPU is composed of bits, that the CPU can shift, or add, etc. In Ceptr, we build semantic trees out of named structures, that themselves are compositions of other semantic trees. 
>
> In traditional computing, which is built on linear sequences of these "words" we're always serializing and "re-hydrating," we rebuild objects from serializations. We lex & parse our programs into syntax trees to compile or interpret them. In Ceptr we keep meaning and structure connected with the values at the very base level.

Semtrex is a formal technique similar to [Regex](https://en.wikipedia.org/wiki/Regular_expression) (regular expressions, for one-dimensional strings of text), but pattern  matching meaning/semantics against literal values in addition to data structures, semantic symbols and protocols (values, symbols and syntax). This allows for writing scripts that trigger actions when matching on a given signal or a message - a key component for building bio-inspired (cell-like, receptors and membranes) computational models.  

![](https://i.imgur.com/wuwxmPY.png)

*Semantic tree structure.*

The concept of the [semantic web](https://en.wikipedia.org/wiki/Semantic_Web) itself has been around for some time, defined by the W3C (World Wide Web Consortium) as providing of *"a common framework that allows data to be shared and reused across application, enterprise, and community boundaries."* Ceptr takes this a step further, occupying a territory of a field known as [ontology engineering](https://en.wikipedia.org/wiki/Ontology_engineering) - the building of formal representations of a set of concepts within a domain and the relationships between those concepts (e.g., in fields and domains such as biology, physics, neuroscience, etc.)

One arbitrary example that might be helpful in illustrating the purpose and application of such semantic framework could be [Seshat](http://seshatdatabank.info/), an academic global history databank used for academic research to do with matters relating to the development of complex societies (rise and fall of empires, boom and bust cycles, etc.) and mapping of historical processes and cycles. As the databank builds up, so does the development of support for diverse interpretative frameworks to the underlying data (supporting, for example, multiple different views of history, particular methodologies and other related domain expertise) which adds more information to the system, gradually revealing more correlations between variables and co-evolving factors with further increased precision and certainty. The [paper](https://escholarship.org/uc/item/9qx38718) ("Seshat: The Global History Databank") concludes:

> Despite the current excitement associated with the digital humanities, historians and social scientists have not really begun to utilize the full power of what modern Information Technology can deliver. **We believe that the new IT capabilities will eventually (and in the not-too-distant future) transform the field of historical social sciences into what the sociologist Randall Collins termed rapid-discovery science** (Collins 1994, although it should be noted that Collins himself was sceptical that such transformation is likely). It is our hope that Seshat: the Global History Databank will be one of the key mechanisms by which such a transformation will be effected.

Or, as with [Martin Armstrong](https://en.wikipedia.org/wiki/Martin_A._Armstrong)'s [Socrates](https://www.ask-socrates.com) platform (which offers "unique perspective and tools intended to help individuals and organizations better research and interpret the global economic and political environment") and his ECM ([Economic Confidence Model](https://www.armstrongeconomics.com/models/7219-2/)), the uncanny precision in forecasting macro-economic and political events of which is widely known - different market cycles are observed simultaneously and at the same time with international capital flows. Zooming out and framing things both locally and globally at the same time, while also not losing sight of the historical past converges in such a way that it immediately reveals things previously hidden and the faulty reasoning that static models combined with only partial information and insufficient knowledge often result in.

By setting up a general computational framework capable of incorporating all kinds of diverse data flows, structures and frameworks (e.g., analytical, statistical, etc.)  in an open DHT-verse of constantly recorded trails of activity and interactions and being able to easily pull and bridge between different fields/disciplines, translating between them while further expanding upon available methodologies, perspectives and ways in which data is seen and contextualized from different divergent angles, etc. ("flows") - this could lay a fruitful ground for new, trans-disciplinary forms of knowledge and collaboration previously unimaginable. 

As the system branches and expands and more people, organizations and institutions contribute, make use of, experiment with and enrich it, more variables and indicators enter, novel associative connections emerge and a more fluid sense of how things work in motion develops. Ceptr could easily incorporate wealths of already available data, knowledge bases and information and combine it with other flows in motion, similarly giving rise to such ubiquitous computation platforms and apps as an open public service and space for collaborative efforts and storage of validated, structured data.

## Forming hApp Ecosystem and Partnerships/Associations 

*"A creator is someone who creates their own impossibilities, and thereby creates possibilities."*

- Gilles Deleuze

A number of interesting initiatives and projects are slowly forming around Holochain and Holo, along with partnerships indicative of the direction of development. Mozilla’s Chief Financial Officer, [Jim Cook](https://mozillians.org/en-US/u/jcook/) has been supportive of Holochain and its agent-centric model, saying that “Holochain is talking Mozilla’s language.” Other projects, like [DAOstack](https://daostack.io), have drawn inspiration from Holochain's model in applying scalable forms of social consensus (i.e., "holographic consensus") between the agencies of different DAOs on the Ethereum blockchain.

Another major [partnership](https://files.holo.host/2018/06/Promether_Partnership_Announcement.pdf) was formed with [Promether](https://promether.com/) - an **Adaptive Symbiotic Platform** (ASP) that implements all the networking, security, and anonymization functionality and modules that applications need to protect their data (described in more detail in their lengthy [white paper]( https://promether.com/docs/Promether-Whitepaper.pdf)). The strategic partnership, based on mutual interests in each other's platforms from a development perspective, has Promether initially providing Holo with exclusive access to alpha/beta testing of the secure communication app (the first Promether-powered app), while Holochain will provide an adaptable platform for P2P apps within Promether’s secure endpoints.

Below are some other projects beginning to develop around and build upon the Holochain foundation and philosophy. And as the ecosystem expands, so do the possibilities of creatively building composable applications from the rich pool of what is available. The Synthetic-Collective Intelligence and sense-making at scale being the emergent properties of this expansion (emergence is a defining property of [complex adaptive systems](https://en.wikipedia.org/wiki/Complex_adaptive_system)).

![](https://i.imgur.com/Y8EuQf4.png)

*A list of applications Holochain, as framework, is best suited for.*

### Sacred Capital: Portable Reputation Across Ecosystems

[Sacred Capital](https://www.sacred.capital/), a Singapore-based startup, takes the idea of reputational currency as value and works to provide Reputation Interchange across different ecosystems, allowing that those reputations be ported and 'staked' across systems, creating feedback loops of reinforcement of desirable behaviors. Essentially, this isn't so much about "monetizing" reputation as such per se, but rather to do with giving reputation money-like qualities or defining reputation as a form of wealth.

### Ulex: A Non-State/Non-Governmental Legal System

[Ulex](https://github.com/proftomwbell/Ulex) is an open-source legal system of [polycentric law](https://en.wikipedia.org/wiki/Polycentric_law) for special zones and jurisdictions (e.g., digital communities, special economic zones, distributed crypto-economies, online p2p markets, etc.) Holochain appears to be ideally suited for the needs of such decentralized legal system.

### Omni Project: Scholarly and Academic Publishing

*"The sciences of today are business enterprises run on business principles. Research in large institutes is not guided by Truth and Reason but by the most rewarding fashion, and the great minds of today increasingly turn to where the money is - which means military matters."*

*"Yes, the academic world is screwed up, and there is nothing you can do about it. But don't worry about that. Just do what you want. If you know what you want to do and advocate for it, no one will put any energy into stopping you."*

- Paul Feyerabend

The distribution of research has become firmly interwoven with various commercial interests and the increasing influence and authority of reputation in academia. The [Omni project](https://github.com/OmniProject/omni) aims to break this deadlock by disengaging research output from profit and rank of status. The best way to achieve this is by providing academics the tools to collectively build an alternative model from the ground-up, which can allow a fundamentally different, more sustainable system that is not bogged down by misalignment of interests and/or subordinate to financial and personal interests to emerge.

Omni is not a journal, repository or a publisher, but rather a public digital space, a kind of "scholarly commons" for academics sharing their work without barriers, quickly reaching their intended audiences and receiving valuable feedback. 

More detailed information about the project can be found [here](https://www.notion.so/The-Omni-Project-a3c36437797149b19a2d8eafe7b3dc23).

### Junto: Censorship-Resistant, Agent-Centric Social Networking 

[Junto](https://junto.foundation/) is a non-profit initiative dedicated to reinventing healthier forms of social networking, not susceptible to political and profit-driven manipulation, but fostering more authentically human atmosphere free from the pollution and toxicity that has come to increasingly define social networking platforms such as Facebook and Twitter.

A Medium post entitled ["The Medium is the Message"](https://medium.com/juntolove/the-medium-is-the-message-644837313afb) (a reference to Marshall McLuhan) outlines the Junto project's design philosophy and purpose:

> The evolution of social media lies in shifting the current nature of interactions. We believe the forms we communicate through are just as important as the message itself.

Other initiatives include a [distributed, holographic Reddit](https://github.com/MightyAlex200/Comet) (ending moderator abuse, Sybil attacks and counting of votes as objective indicators), a [customizable dashboard](https://core.network/) for integrating all social networking apps that allows for better tracking of impact, influence, developing learning capacities and building communities and their respective currencies, and many more along those lines.

## Further Implications and Philosophical Underpinnings

*"Societies have always been shaped more by the nature of the media by which men communicate than by the content of the communication."*

- Marshall McLuhan

Founding member and Holo.Host CEO [Arthur Brock](https://twitter.com/artbrock) writes in a [blog post](http://www.artbrock.com/blog/designing-social-flows-chapter-6-designing-incentives) on designing social flows:

> *How is “awareness” wired into organizations?  Through the currencies we create as shared symbol systems to shape, enable and measure value flows (Think “Current-Sees” to keep in mind they’re not just money.). These currencies form the nervous system of a social organism, and they are the best way to observe and to modify its pattern of awareness.*
>
> *As humans, we know that people are born and that they die, but as far as the government is concerned, citizens are issued through birth certificates and expired through death certificates -- and a government’s systems are designed to service citizens. A government service literally cannot “see” you if you don’t show up in the currencies by which the flow of services are managed.*

The implications of this capability to generate globally visible patterns should be evident. Historically, the emergence of information systems of symbolic representation, forms of writing, bureaucracy and record-keeping are among the categories of variables defining social complexity and the trajectories of cultural evolution (which biological evolution tends to follow). As the Ceptr [paper](http://ceptr.org/whitepapers/grammatics) on Grammatic Capacities states: 

> The fundamental insight comes from the observation that new complex adaptive systems, as well as fundamental changes within those systems always appear concomitant with the emergence of a special type of informational infrastructure. We call such an infrastructure a Grammatic Capacity and propose a formalism to describe them abstractly, as well as offer a proof-of-concept new Grammatic Capacity for catalyzing change in the complex adaptive system we call human society.

[Edmund Berger](https://twitter.com/EBBerger) goes on to expand upon Deleuze & Guattari's concept of "schizoanalysis" as, among other things, a critique of psychoanalysis, shedding further light on the matter from the angle of Guattari's further work where he emphasizes the ecological approach and ecological scales in framing our socio-technical world (drawing also from the work of Gregory Bateson, which very much overlaps with the Holochain underlying philosophy of Holochain and Ceptr). It is worth citing the blog post (["How does  Schizoanalysis Work?"](https://deterritorialinvestigations.wordpress.com/2013/05/15/how-does-schizoanalysis-work-or-how-do-you-make-a-class-operate-like-a-work-of-art/)), which strikingly relates to Holochain and what it aims to build and provide us with in the future on the horizon:

> ![](https://i.imgur.com/ER9lbPp.png)
>
> ​                *Guattari's four-dimensional schizoanalytic cartrography.*
>
> In the upper left quadrant there is the “machinic phylum,” the space of knowledge and ideas, rhizomatic wanderings and the application of creative desiring-flows. If this area is machinic, it is because Guattari always wrote with one foot in the future; moving forward in time, the nature of knowledge and how it is applied will always take on more and more technological and computational relations. I would argue that the machinic phylum is synonymous with the General Intellect identified by Marx and elaborated to a higher degree by the Italian Autonomists. Knowledge is a social body, owned by no individual, and like desire (especially like desire!) it moves in flows, it makes new conjunctions and evolves into higher and higher planes. It does not have to be technical knowledge, but any form of knowledge or flight of ideas that is produced, put out into the world, and used by others to build upon.
>
> The positioning of each space in the cartography shows how one relates to the next, first with how the two on the left-hand side couple with each other, just as the ones of the right do the same. At the same time, there is an explicit relationship between the two across the top, as there are across the bottom. **The common linkage between the incorporeal universes and the machinic phylum is that what we could call ‘inspiration,’ a catalyst for knowledge, born from the images and sensations when we have encounters or experiences. Thus there exists a kind of feedback loop between the two: manifestations of the phylum trigger responses in our incorporeal universes, which in turn can add to the social knowledge body or General Intellect. Likewise, it takes various flows (money flows, language flows, genetic flows, commodity flows) to build up an existential territory; no territory comes into being spontaneously. The existential territory is like Wiener’s idea of the enclave from entropy that fosters the creation of life.**
>
> [...]
>
> **From this view, Guattari posed his idea of “ecosophy,” a revitalization of ecology to encompass the whole dynamic world of flows. This ecosophic model is itself composed of three ecological scales (first proposed in the 1970s by Gregory Bateson): the mind, the society, and the environment. The stratification of each as a separate entity, however, is misleading; following the ongoing discourse started in conjunction with Deleuze, the three scales are indistinguishable from one to the next. Environment shapes the mind, the mind shapes society, society shapes the environment, society shapes the mind, and so on. “Environment” need not only be the standard eco-system environment that we traditionally understand it to be; like Marshall McLuhan, Guattari understood that technology and the media platforms it generates (radio, television, and later, the internet) shapes the social environment and reorganizes the way micro and macropolitical change can occur. The mind itself, drawing on Bateson, operates in its own ecology, as does the incorporeal shifts and manifestations that arise within the mind in relation to external factors. “Now more than ever,” he writes, “nature cannot be separated from culture; in order to comprehend eco-systems, the mechanosphere, and the social and individual Universes of reference, we must learn to think ‘transversally’.”**

All this is obviously a radical departure from the widely held views and perceptions of "cryptocurrencies" and what constitutes value in society, such that it catalyzes emergent systemic patterns of behavior (i.e., social coherence) by facilitating apparently meaningful collaboration of components (individuals) in order to show capabilities of the overall system (far) beyond the capabilities of the individual components.

>  *"The rhizome pertains to a map that is always detachable, connectible, reversible, modifiable, and has multiple entryways and exits and its own lines of flight."* 
>
> - Deleuze and Guattari, 1987.

It might be helpful to try and better elucidate the Deleuzian concept of the "rhizome" at this point. Deleuze and Guattari use the terms "rhizome" and "rhizomatic" to describe theory and research allowing for multiple, non-hierarchical entry and exit points in data representation and interpretation. A rhizome works with planar and trans-species connections (in contrast with vertical and linear connections). Examples of [mutualism](https://en.wikipedia.org/wiki/Mutualism_(biology) ) in biology are given (the orchid and the wasp), where two different species form a [multiplicity](https://en.wikipedia.org/wiki/Multiplicity_(philosophy) ) (i.e., a unity that is multiple in itself, across different dimensions and domains) as they interact. Or [horizontal gene transfer](https://en.wikipedia.org/wiki/Horizontal_gene_transfer) and [hybridization](https://en.wikipedia.org/wiki/Hybridisation_(biology) ). 

> **"As a model for culture, the rhizome resists the organizational structure of the root-tree system which charts causality along chronological lines and looks for the original source of 'things' and looks towards the pinnacle or conclusion of those 'things.' A rhizome, on the other hand, is characterized by 'ceaselessly established connections between semiotic chains, organizations of power, and circumstances relative to the arts, sciences, and social struggles.' Rather than narrativize history and culture, the rhizome presents history and culture as a map or wide array of attractions and influences with no specific origin or genesis, for a 'rhizome has no beginning or end; it is always in the middle, between things, interbeing, intermezzo.' The planar movement of the rhizome resists chronology and organization, instead favoring a nomadic system of growth and propagation.**

![](https://i.imgur.com/pddULVs.jpg)

Holochain thus puts emphasis on the nature of the medium, in the [McLuhan](https://en.wikipedia.org/wiki/Marshall_McLuhan) sense of how the medium of technology shapes the perception of reality. His famous phrase, "the medium is the message" (and how "the message has as much significance as the graffiti on the outside of the atom bomb"), is intended to shock into realizing that the form of the medium/technology embeds itself in any message it would transmit or convey, creating a symbiotic relationship whereby  the medium influences how the message is perceived.

Additionally, centralized control frequently involves deliberate manipulation of the medium so that it would project a falsified/distorted perception of reality (e.g., Facebook's psychological profiling and targeted machine learning persuasion aimed at one's own beliefs about the world, the "fake news" phenomena, politically motivated tailoring of search algorithms, etc.) Ceptr is a proposition for another vision of the Internet, structured around Holochain as an **unencloseable carrier** for direct peer-to-peer communication that evades centralized structures and control.  

![](https://i.imgur.com/OLrsY7s.png)

*Marshall McLuhan, from the introductory chapters of "Laws of Media - The New Science."*

## Conclusion and Summary

Holochain and the grand plan of Ceptr stand out among the most innovative/original, ambitious, unique and carefully thought through undertakings (as immediately noticed by the careful choice of words and terminology, as well as the sense of distance from the prevailing miasma of hype and fraud in the midst of an unregulated and oversold tech boom) in the realm of distributed systems crypto-economies. Unlike the vast majority of blockchain-based systems, many of which defined by a centralizing trajectory/pull under the guise of social movements and decentralization initiatives and trying hard to come up with the "next big thing", Ceptr is a project with a clear vision of purpose - one also driven by an undercurrent of historical necessity in the phase transition we find ourselves at. 

Perhaps the only other project Ceptr/Holochain comes close to in a way that a certain comparison can be drawn is IOTA, in the sense of how both constitute efforts at laying the groundwork and foundations for evolving complex adaptive systems addressing the real issues and problems we, as technological societies in a globalized world, are facing on the horizon. Also, neither (of the two) employs a blockchain architecture or has any form of enforced global consensus. IOTA, however, is rather geared towards the future landscape of interconnected IoT devices and meshnets of a near future machine-to-machine economy (and as such, the interfacing human agent is more of an afterthought, rather than center of focus), while Holochain is on the other hand conceived as technology for fueling sophisticated social applications, facilitating social organization, collaboration and collective-sense making (or, also, as a framework for building commons and meeting fundamental human needs). Said otherwise and in summary, if IOTA is busy with engineering the basis for distributed Artificial-Machine Intelligence, Ceptr is rather geared towards Synthetic-Collective Intelligence.

## Links and Resources

Public (Mattermost) [chat](https://chat.holochain.net/).

Eric Harris-Braun's [blog](http://eric.harris-braun.com/blog/).

Arthur Brock's [blog](http://www.artbrock.com/blog/).

Holochain [official site](https://holochain.org) and [subreddit](https://www.reddit.com/r/holochain).

Ceptr [official site](http://ceptr.org).

The Metacurrency project [official site](http://metacurrency.org).

Twitter [account](https://twitter.com/holochain).

Developer [documentation](https://developer.holochain.org/).

[Medium](https://medium.com/@holochain).
