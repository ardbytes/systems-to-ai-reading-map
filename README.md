# Zero to Pro Engineer

**112 topics from 8 of the most widely read engineering books, in the order you'd learn them.**

From how a CPU runs your code, to operating systems, distributed data, system design, reliability, ML systems, and building and shipping LLMs.

Every topic below is a real chapter or section of its book, with the exact chapter number, so you can open the book and go straight to it. Where the authors publish the material for free, the topic links straight to it.

## How to use this

- **Go in order.** Each stage builds on the one before it. Topic 1 is bits and bytes; topic 112 is shipping AI products.
- **One topic at a time.** Read the chapter, then explain it to someone (or write it down) without looking.
- **Use the free links.** OSTEP and the Google SRE book are completely free, by their authors. The LLM book's code is free on GitHub.
- **Buy or borrow the rest.** These books are worth owning. The links go to the official pages.

## The 8 books

| # | Stage | Book | Author(s) | Free? |
|---|---|---|---|---|
| 1 | The Machine | [Computer Systems: A Programmer's Perspective](https://csapp.cs.cmu.edu/3e/about.html) (3rd ed.) | Randal E. Bryant, David R. O'Hallaron | — |
| 2 | The Operating System | [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/) | Remzi & Andrea Arpaci-Dusseau | Free online, by the authors |
| 3 | Data Systems | [Designing Data-Intensive Applications](https://www.oreilly.com/library/view/designing-data-intensive-applications/9781098119058/) (2nd ed.) | Martin Kleppmann, Chris Riccomini | — |
| 4 | System Design | [System Design Interview: An Insider's Guide, Vol. 1](https://bytebytego.com/) | Alex Xu | — |
| 5 | Reliability | [Site Reliability Engineering](https://sre.google/sre-book/table-of-contents/) | Betsy Beyer, Chris Jones, Jennifer Petoff, Niall Richard Murphy (Google) | Free online, by Google |
| 6 | ML Systems | [Designing Machine Learning Systems](https://github.com/chiphuyen/dmls-book) | Chip Huyen | Chapter summaries & resources on the author's GitHub |
| 7 | LLMs from Scratch | [Build a Large Language Model (From Scratch)](https://github.com/rasbt/LLMs-from-scratch) | Sebastian Raschka | All code & notebooks free on the author's GitHub |
| 8 | AI Engineering | [AI Engineering: Building Applications with Foundation Models](https://github.com/chiphuyen/aie-book) | Chip Huyen | Table of contents & resources on the author's GitHub |

## Stage 1 · The Machine

*[Computer Systems: A Programmer's Perspective](https://csapp.cs.cmu.edu/3e/about.html), 3rd ed.*: How code actually runs: bits, assembly, memory, linking, I/O.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 1 | Bits, bytes & integers | Ch. 2 (§2.1–2.3) | — |
| 2 | IEEE floating point | §2.4 | — |
| 3 | x86-64 assembly | Ch. 3 | — |
| 4 | Procedures & the run-time stack | §3.7 | — |
| 5 | Buffer overflow attacks | §3.10.3–3.10.4 | — |
| 6 | Pipelining (Y86-64) | §4.4–4.5 | — |
| 7 | The memory hierarchy | Ch. 6 | — |
| 8 | Locality & cache memories | §6.2, §6.4–6.5 | — |
| 9 | Linking: static vs dynamic | Ch. 7 (§7.2, §7.10) | — |
| 10 | Exceptions & signals | Ch. 8 (§8.1, §8.5) | — |
| 11 | Dynamic memory allocation | §9.9 | — |
| 12 | System-level I/O | Ch. 10 | — |
| 13 | Internet basics: IP, DNS, HTTP | §11.3, §11.5 | — |
| 14 | The sockets interface | §11.4 | — |

## Stage 2 · The Operating System

*[Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/)*: Processes, memory, concurrency and file systems, from first principles.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 15 | Processes | Ch. 4 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-intro.pdf) |
| 16 | Process API: fork / exec / wait | Ch. 5 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-api.pdf) |
| 17 | System calls & traps | Ch. 6 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf) |
| 18 | Limited direct execution | Ch. 6 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf) |
| 19 | Scheduling: MLFQ & lottery | Ch. 7–9 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-sched-mlfq.pdf) |
| 20 | Address spaces | Ch. 13 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-intro.pdf) |
| 21 | Paging & TLBs | Ch. 18–19 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-paging.pdf) |
| 22 | Swapping: mechanisms & policies | Ch. 21–22 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-beyondphys.pdf) |
| 23 | Threads | Ch. 26 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-intro.pdf) |
| 24 | Locks | Ch. 28 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-locks.pdf) |
| 25 | Condition variables & semaphores | Ch. 30–31 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-cv.pdf) |
| 26 | Concurrency bugs & deadlock | Ch. 32 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-bugs.pdf) |
| 27 | File systems: inodes & journaling | Ch. 40, 42 | [Read](https://pages.cs.wisc.edu/~remzi/OSTEP/file-implementation.pdf) |

## Stage 3 · Data Systems

*[Designing Data-Intensive Applications](https://www.oreilly.com/library/view/designing-data-intensive-applications/9781098119058/), 2nd ed.*: Storage, replication, sharding, transactions and consensus: the backbone of every backend.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 28 | Trade-offs in data systems architecture | Ch. 1 | — |
| 29 | Defining nonfunctional requirements | Ch. 2 | — |
| 30 | Data models: SQL, document, graph | Ch. 3 | — |
| 31 | Storage: LSM-trees vs B-trees | Ch. 4 | — |
| 32 | Encoding & schema evolution | Ch. 5 | — |
| 33 | Replication: leader, multi, leaderless | Ch. 6 | — |
| 34 | Sharding | Ch. 7 | — |
| 35 | Transactions & isolation levels | Ch. 8 | — |
| 36 | Trouble with distributed systems | Ch. 9 | — |
| 37 | Consistency & consensus | Ch. 10 | — |
| 38 | Batch processing | Ch. 11 | — |
| 39 | Stream processing | Ch. 12 | — |
| 40 | A philosophy of streaming systems | Ch. 13 | — |
| 41 | Doing the right thing | Ch. 14 | — |

## Stage 4 · System Design

*[System Design Interview: An Insider's Guide, Vol. 1](https://bytebytego.com/)*: Turning the theory into real designs: rate limiters, feeds, chat, video, storage.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 42 | Scale from zero to millions of users | Ch. 1 | — |
| 43 | Back-of-the-envelope estimation | Ch. 2 | — |
| 44 | Framework for system design interviews | Ch. 3 | — |
| 45 | Rate limiter | Ch. 4 | — |
| 46 | Consistent hashing | Ch. 5 | — |
| 47 | Key-value store | Ch. 6 | — |
| 48 | Unique ID generator | Ch. 7 | — |
| 49 | URL shortener | Ch. 8 | — |
| 50 | Web crawler | Ch. 9 | — |
| 51 | Notification system | Ch. 10 | — |
| 52 | News feed system | Ch. 11 | — |
| 53 | Chat system | Ch. 12 | — |
| 54 | Search autocomplete | Ch. 13 | — |
| 55 | Design YouTube | Ch. 14 | — |
| 56 | Design Google Drive | Ch. 15 | — |

## Stage 5 · Reliability

*[Site Reliability Engineering](https://sre.google/sre-book/table-of-contents/)*: Keeping systems up: SLOs, error budgets, on-call, incidents, overload.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 57 | Embracing risk & error budgets | Ch. 3 | [Read](https://sre.google/sre-book/embracing-risk/) |
| 58 | SLIs, SLOs & SLAs | Ch. 4 | [Read](https://sre.google/sre-book/service-level-objectives/) |
| 59 | Eliminating toil | Ch. 5 | [Read](https://sre.google/sre-book/eliminating-toil/) |
| 60 | The four golden signals | Ch. 6 | [Read](https://sre.google/sre-book/monitoring-distributed-systems/) |
| 61 | Release engineering | Ch. 8 | [Read](https://sre.google/sre-book/release-engineering/) |
| 62 | Being on-call | Ch. 11 | [Read](https://sre.google/sre-book/being-on-call/) |
| 63 | Effective troubleshooting | Ch. 12 | [Read](https://sre.google/sre-book/effective-troubleshooting/) |
| 64 | Managing incidents | Ch. 14 | [Read](https://sre.google/sre-book/managing-incidents/) |
| 65 | Postmortem culture | Ch. 15 | [Read](https://sre.google/sre-book/postmortem-culture/) |
| 66 | Testing for reliability | Ch. 17 | [Read](https://sre.google/sre-book/testing-reliability/) |
| 67 | Load balancing in the datacenter | Ch. 20 | [Read](https://sre.google/sre-book/load-balancing-datacenter/) |
| 68 | Handling overload | Ch. 21 | [Read](https://sre.google/sre-book/handling-overload/) |
| 69 | Addressing cascading failures | Ch. 22 | [Read](https://sre.google/sre-book/addressing-cascading-failures/) |

## Stage 6 · ML Systems

*[Designing Machine Learning Systems](https://github.com/chiphuyen/dmls-book)*: ML as an engineering discipline: data, features, deployment, drift, monitoring.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 70 | ML in research vs production | Ch. 1 | — |
| 71 | Data engineering fundamentals | Ch. 3 | — |
| 72 | Sampling & labeling | Ch. 4 | — |
| 73 | Class imbalance | Ch. 4 | — |
| 74 | Feature engineering | Ch. 5 | — |
| 75 | Data leakage | Ch. 5 | — |
| 76 | Model development & ensembles | Ch. 6 | — |
| 77 | Model offline evaluation | Ch. 6 | — |
| 78 | Batch vs online prediction | Ch. 7 | — |
| 79 | Data distribution shifts | Ch. 8 | — |
| 80 | Monitoring & observability | Ch. 8 | — |
| 81 | Continual learning | Ch. 9 | — |
| 82 | Test in production: shadow, A/B, canary | Ch. 9 | — |
| 83 | ML platform & feature store | Ch. 10 | — |

## Stage 7 · LLMs from Scratch

*[Build a Large Language Model (From Scratch)](https://github.com/rasbt/LLMs-from-scratch)*: Build a GPT yourself: tokenizer, attention, training, finetuning.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 84 | Tokenization & byte pair encoding | §2.2, §2.5 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch02) |
| 85 | Token embeddings & word positions | §2.7–2.8 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch02) |
| 86 | Data sampling with a sliding window | §2.6 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch02) |
| 87 | Self-attention | §3.3–3.4 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch03) |
| 88 | Causal attention | §3.5 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch03) |
| 89 | Multi-head attention | §3.6 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch03) |
| 90 | LayerNorm, GELU & shortcut connections | §4.2–4.4 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch04) |
| 91 | The transformer block | §4.5 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch04) |
| 92 | Coding the GPT model | §4.6 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch04) |
| 93 | Decoding: temperature & top-k | §5.3 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch05) |
| 94 | Training loop: autograd & AdamW | §5.2, App. A | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/appendix-A) |
| 95 | Pretraining & cross-entropy loss | §5.1–5.2 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch05) |
| 96 | Loading pretrained weights | §5.5 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch05) |
| 97 | Finetuning for classification | Ch. 6 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch06) |
| 98 | Finetuning to follow instructions | Ch. 7 | [Read](https://github.com/rasbt/LLMs-from-scratch/tree/main/ch07) |

## Stage 8 · AI Engineering

*[AI Engineering: Building Applications with Foundation Models](https://github.com/chiphuyen/aie-book)*: Shipping on top of foundation models: evaluation, prompting, RAG, agents, finetuning, inference.

| # | Topic | Where in the book | Free read |
|---|---|---|---|
| 99 | Foundation models: data, modeling, size | Ch. 2 | — |
| 100 | Sampling strategies | Ch. 2 | — |
| 101 | Evaluation & AI as a judge | Ch. 3–4 | — |
| 102 | Prompt engineering | Ch. 5 | — |
| 103 | Prompt injection & defenses | Ch. 5 | — |
| 104 | RAG & retrieval optimization | Ch. 6 | — |
| 105 | Embeddings & vector search | Ch. 3, 6 | — |
| 106 | Agents: tools & planning | Ch. 6 | — |
| 107 | Memory | Ch. 6 | — |
| 108 | Parameter-efficient finetuning | Ch. 7 | — |
| 109 | Dataset engineering & synthesis | Ch. 8 | — |
| 110 | Inference optimization | Ch. 9 | — |
| 111 | Guardrails, model router & gateway | Ch. 10 | — |
| 112 | User feedback | Ch. 10 | — |

## Contributing

Found a better free official resource for a topic, or a wrong chapter number? Open an issue or a pull request. Please keep links to the authors' or publishers' own material.

## License

The topic list is [MIT licensed](LICENSE). The books belong to their authors and publishers; this repo only points to them.
