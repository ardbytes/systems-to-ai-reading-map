# Systems to AI: A Reading Map

**132 topics from 14 well-known engineering books, in a suggested reading order.**

From how a CPU runs your code, to operating systems, networking, distributed data, system design, APIs, containers, reliability, the math behind ML, ML systems, and building and shipping LLMs.

Every topic below is a real chapter or section of its book.

## How to use this

- **Go in order.** Each stage builds on the one before it. Topic 1 is bits and bytes; topic 132 is shipping AI products.
- **One topic at a time.** Read the chapter, then explain it to someone (or write it down) without looking.
- **Start with what's free.** OSTEP, the Google SRE book and the Deep Learning book are free to read online, by their authors. The LLM book's code is free on GitHub.
- **Buy or borrow the rest.** These books are worth owning. The links go to the official pages.

## The 14 books

| # | Stage | Book | Author(s) | Free? |
|---|---|---|---|---|
| 1 | The Machine | [Computer Systems: A Programmer's Perspective](https://csapp.cs.cmu.edu/3e/about.html) (3rd ed.) | Randal E. Bryant, David R. O'Hallaron | — |
| 2 | The Operating System | [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/) | Remzi & Andrea Arpaci-Dusseau | Free online, by the authors |
| 3 | Networking | [Computer Networking: A Top-Down Approach](https://gaia.cs.umass.edu/kurose_ross/index.php) (9th ed.) | James F. Kurose, Keith W. Ross | — |
| 4 | Data Systems | [Designing Data-Intensive Applications](https://www.oreilly.com/library/view/designing-data-intensive-applications/9781098119058/) (2nd ed.) | Martin Kleppmann, Chris Riccomini | — |
| 5 | System Design | [System Design Interview: An Insider's Guide, Vol. 1](https://bytebytego.com/) | Alex Xu | — |
| 6 | Services & APIs | [Building Microservices](https://samnewman.io/books/building_microservices_2nd_edition/) (2nd ed.) | Sam Newman | — |
| 7 | Containers | [Docker Deep Dive](https://leanpub.com/dockerdeepdive) | Nigel Poulton | — |
| 8 | Orchestration | [Kubernetes: Up and Running](https://www.oreilly.com/library/view/kubernetes-up-and/9781098110192/) (3rd ed.) | Brendan Burns, Joe Beda, Kelsey Hightower, Lachlan Evenson | — |
| 9 | Infrastructure as Code | [Terraform: Up & Running](https://www.terraformupandrunning.com/) (3rd ed.) | Yevgeniy Brikman | — |
| 10 | Reliability | [Site Reliability Engineering](https://sre.google/sre-book/table-of-contents/) | Betsy Beyer, Chris Jones, Jennifer Petoff, Niall Richard Murphy (Google) | Free online, by Google |
| 11 | Math for ML | [Deep Learning](https://www.deeplearningbook.org/) | Ian Goodfellow, Yoshua Bengio, Aaron Courville | Free to read online, by the authors |
| 12 | ML Systems | [Designing Machine Learning Systems](https://github.com/chiphuyen/dmls-book) | Chip Huyen | Chapter summaries & resources on the author's GitHub |
| 13 | LLMs from Scratch | [Build a Large Language Model (From Scratch)](https://github.com/rasbt/LLMs-from-scratch) | Sebastian Raschka | All code & notebooks free on the author's GitHub |
| 14 | AI Engineering | [AI Engineering: Building Applications with Foundation Models](https://github.com/chiphuyen/aie-book) | Chip Huyen | Table of contents & resources on the author's GitHub |

## Stage 1 · The Machine

*[Computer Systems: A Programmer's Perspective](https://csapp.cs.cmu.edu/3e/about.html), 3rd ed.*: How code actually runs: bits, assembly, memory, linking, I/O.

| # | Topic |
|---|---|
| 1 | Bits, bytes & integers |
| 2 | IEEE floating point |
| 3 | x86-64 assembly |
| 4 | Procedures & the run-time stack |
| 5 | Buffer overflow attacks |
| 6 | Pipelining (Y86-64) |
| 7 | The memory hierarchy |
| 8 | Locality & cache memories |
| 9 | Linking: static vs dynamic |
| 10 | Exceptions & signals |
| 11 | Dynamic memory allocation |
| 12 | System-level I/O |
| 13 | The sockets interface |

## Stage 2 · The Operating System

*[Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/)*: Processes, memory, concurrency and file systems, from first principles.

| # | Topic |
|---|---|
| 14 | Processes |
| 15 | Process API: fork / exec / wait |
| 16 | System calls & traps |
| 17 | Limited direct execution |
| 18 | Scheduling: MLFQ & lottery |
| 19 | Address spaces |
| 20 | Paging & TLBs |
| 21 | Swapping: mechanisms & policies |
| 22 | Threads |
| 23 | Locks |
| 24 | Condition variables & semaphores |
| 25 | Concurrency bugs & deadlock |
| 26 | File systems: inodes & journaling |

## Stage 3 · Networking

*[Computer Networking: A Top-Down Approach](https://gaia.cs.umass.edu/kurose_ross/index.php), 9th ed.*: How data actually crosses the internet: layers, HTTP, DNS, TCP/UDP, IP, TLS.

| # | Topic |
|---|---|
| 27 | Internet & protocol layers |
| 28 | HTTP |
| 29 | DNS |
| 30 | TCP vs UDP & congestion control |
| 31 | IP addressing & NAT |
| 32 | A day in the life of a web page request |
| 33 | TLS & network security |

## Stage 4 · Data Systems

*[Designing Data-Intensive Applications](https://www.oreilly.com/library/view/designing-data-intensive-applications/9781098119058/), 2nd ed.*: Storage, replication, sharding, transactions and consensus: the backbone of every backend.

| # | Topic |
|---|---|
| 34 | Trade-offs in data systems architecture |
| 35 | Defining nonfunctional requirements |
| 36 | Data models: SQL, document, graph |
| 37 | Storage: LSM-trees vs B-trees |
| 38 | Encoding & schema evolution |
| 39 | Replication: leader, multi, leaderless |
| 40 | Sharding |
| 41 | Transactions & isolation levels |
| 42 | Trouble with distributed systems |
| 43 | Consistency & consensus |
| 44 | Batch processing |
| 45 | Stream processing |
| 46 | Doing the right thing |

## Stage 5 · System Design

*[System Design Interview: An Insider's Guide, Vol. 1](https://bytebytego.com/)*: Turning the theory into real designs: rate limiters, feeds, chat, video, storage.

| # | Topic |
|---|---|
| 47 | Scale from zero to millions of users |
| 48 | Back-of-the-envelope estimation |
| 49 | Framework for system design interviews |
| 50 | Rate limiter |
| 51 | Consistent hashing |
| 52 | Key-value store |
| 53 | Unique ID generator |
| 54 | URL shortener |
| 55 | Web crawler |
| 56 | Notification system |
| 57 | News feed system |
| 58 | Chat system |
| 59 | Search autocomplete |
| 60 | Design YouTube |
| 61 | Design Google Drive |

## Stage 6 · Services & APIs

*[Building Microservices](https://samnewman.io/books/building_microservices_2nd_edition/), 2nd ed.*: How services talk to each other and stay secure.

| # | Topic |
|---|---|
| 62 | Communication styles: sync, async, events |
| 63 | Implementing service communication |
| 64 | Microservice security |

## Stage 7 · Containers

*[Docker Deep Dive](https://leanpub.com/dockerdeepdive)*: Packaging and running software anywhere: images, containers, Compose, networking, volumes.

| # | Topic |
|---|---|
| 65 | Images & containers |
| 66 | Containerizing an app & Compose |
| 67 | Docker networking & volumes |

## Stage 8 · Orchestration

*[Kubernetes: Up and Running](https://www.oreilly.com/library/view/kubernetes-up-and/9781098110192/), 3rd ed.*: Running containers at scale: pods, services, deployments.

| # | Topic |
|---|---|
| 68 | Pods |
| 69 | Service discovery |
| 70 | Deployments |

## Stage 9 · Infrastructure as Code

*[Terraform: Up & Running](https://www.terraformupandrunning.com/), 3rd ed.*: Defining infrastructure in code: why it matters, state, modules.

| # | Topic |
|---|---|
| 71 | Why infrastructure as code |
| 72 | Terraform state & modules |

## Stage 10 · Reliability

*[Site Reliability Engineering](https://sre.google/sre-book/table-of-contents/)*: Keeping systems up: SLOs, error budgets, on-call, incidents, overload.

| # | Topic |
|---|---|
| 73 | Embracing risk & error budgets |
| 74 | SLIs, SLOs & SLAs |
| 75 | Eliminating toil |
| 76 | The four golden signals |
| 77 | Release engineering |
| 78 | Being on-call |
| 79 | Effective troubleshooting |
| 80 | Managing incidents |
| 81 | Postmortem culture |
| 82 | Testing for reliability |
| 83 | Load balancing in the datacenter |
| 84 | Handling overload |
| 85 | Addressing cascading failures |

## Stage 11 · Math for ML

*[Deep Learning](https://www.deeplearningbook.org/)*: The math under every model: linear algebra, probability, optimization, backprop.

| # | Topic |
|---|---|
| 86 | Linear algebra |
| 87 | Probability & information theory |
| 88 | Gradient-based optimization |
| 89 | Feedforward networks & backprop |

## Stage 12 · ML Systems

*[Designing Machine Learning Systems](https://github.com/chiphuyen/dmls-book)*: ML as an engineering discipline: data, features, deployment, drift, monitoring.

| # | Topic |
|---|---|
| 90 | ML in research vs production |
| 91 | Data engineering fundamentals |
| 92 | Sampling & labeling |
| 93 | Class imbalance |
| 94 | Feature engineering |
| 95 | Data leakage |
| 96 | Model development & ensembles |
| 97 | Model offline evaluation |
| 98 | Batch vs online prediction |
| 99 | Data distribution shifts |
| 100 | Monitoring & observability |
| 101 | Continual learning |
| 102 | Test in production: shadow, A/B, canary |
| 103 | ML platform & feature store |

## Stage 13 · LLMs from Scratch

*[Build a Large Language Model (From Scratch)](https://github.com/rasbt/LLMs-from-scratch)*: Build a GPT yourself: tokenizer, attention, training, finetuning.

| # | Topic |
|---|---|
| 104 | Tokenization & byte pair encoding |
| 105 | Token embeddings & word positions |
| 106 | Data sampling with a sliding window |
| 107 | Self-attention |
| 108 | Causal attention |
| 109 | Multi-head attention |
| 110 | LayerNorm, GELU & shortcut connections |
| 111 | The transformer block |
| 112 | Coding the GPT model |
| 113 | Decoding: temperature & top-k |
| 114 | Training loop: autograd & AdamW |
| 115 | Pretraining & cross-entropy loss |
| 116 | Loading pretrained weights |
| 117 | Finetuning for classification |
| 118 | Finetuning to follow instructions |

## Stage 14 · AI Engineering

*[AI Engineering: Building Applications with Foundation Models](https://github.com/chiphuyen/aie-book)*: Shipping on top of foundation models: evaluation, prompting, RAG, agents, finetuning, inference.

| # | Topic |
|---|---|
| 119 | Foundation models: data, modeling, size |
| 120 | Sampling strategies |
| 121 | Evaluation & AI as a judge |
| 122 | Prompt engineering |
| 123 | Prompt injection & defenses |
| 124 | RAG & retrieval optimization |
| 125 | Embeddings & vector search |
| 126 | Agents: tools & planning |
| 127 | Memory |
| 128 | Parameter-efficient finetuning |
| 129 | Dataset engineering & synthesis |
| 130 | Inference optimization |
| 131 | Guardrails, model router & gateway |
| 132 | User feedback |

## Contributing

Spotted a mistake or a topic that belongs here? Open an issue or a pull request.

## License

The topic list is [MIT licensed](LICENSE). The books belong to their authors and publishers; this repo only points to them.
