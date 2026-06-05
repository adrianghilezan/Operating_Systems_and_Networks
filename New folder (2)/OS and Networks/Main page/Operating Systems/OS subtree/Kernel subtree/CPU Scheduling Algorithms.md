# ⏱️ CPU Scheduling Algorithms

> [!NOTE] Architecture Status
> "Current Location: Operating Systems -> Kernel & Process Management -> CPU Scheduling Algorithms"

### 🎯 Core Focus & Definition
> CPU Scheduling Algorithms represent the tactical policy engines used by the kernel to distribute physical processor execution time across competing threads. They determine the exact sequence and duration for which a task controls a CPU core, directly optimizing system throughput, latency, and fairness.

---

### 📌 INTRODUCTION & OVERVIEW
Because physical CPU cores can only execute a single hardware instruction stream at a instant, the operating system must orchestrate an illusion of simultaneous multi-tasking. The CPU scheduler serves as the master decision-maker, handling the rapid context-switching loops of the system. It handles two primary modes of operation: non-preemptive scheduling (where a task keeps control until it voluntarily yields) and preemptive scheduling (where the kernel uses hardware timers to forcibly intercept a running process). The ultimate goal is to balance conflicting metrics, such as minimizing interactive user latency while maximizing background data processing speeds.

---

### ⏳ HISTORICAL CONTEXT & EVOLUTION
* **Batch Processing & Simple Queues:** Early mainframes processed jobs sequentially using simple First-Come, First-Served (FCFS) or Shortest Job First (SJF) non-preemptive algorithms. These models were highly efficient for raw mathematical computations but entirely unusable for interactive user computing.
* **The Multiprogramming Multi-Level Era:** The rise of desktop workstations introduced preemptive time-slicing algorithms like Round Robin (RR) and Multi-Level Feedback Queues (MLFQ). MLFQ dynamically changed task priorities based on behavior, automatically rewarding interactive apps that slept often while restricting CPU-heavy computation loops.
* **Modern Multicore & Fair Schedulers:** Modern enterprise engines utilize highly advanced heuristics like the Linux Completely Fair Scheduler (CFS), which tracks execution using a balanced Red-Black tree structure. Today's schedulers must also calculate CPU cache locality and Energy-Aware Scheduling (EAS) to balance computing loads across heterogeneous mobile processors (like ARM big.LITTLE architectures).

---

### 🔗 INTER-DISCIPLINARY RELATIONS & CONNECTIONS
* **Dependencies (What this specific area needs):**
  * *Computer Architecture:* Deeply relies on high-precision physical hardware timer interrupts to seize control of execution lines and handle asymmetric multicore hardware layout boundaries.
  * *Algorithms & Data Structures:* Requires highly optimized algorithmic topologies, such as balanced trees, priority queues, and bitmapped arrays to execute scheduling lookups in $O(1)$ or $O(\log n)$ operational time.
* **Influences (What this specific area powers):**
  * *Cybersecurity & Cryptographic Defenses:* Scheduling patterns can become highly dangerous side-channel attack vectors. By precisely measuring how long a specific algorithm takes to yield the CPU, an attacker can extract cryptographic keys via scheduling-latency analysis.
  * *Real-Time Embedded Systems:* Critical avionic and automotive execution meshes rely directly on deterministic, hard real-time scheduling policies (like Rate Monotonic or Earliest Deadline First) where missing a single deadline results in catastrophic hardware failure.

---

### 🧠 STRATEGIC PROBLEMS & OPEN CHALLENGES
* **Important Classic Problems:**
  * **The Priority Inversion Disaster:** A critical failure where a low-priority process locks a resource needed by a high-priority task, but a medium-priority task interrupts the low-priority process, starving the critical task indefinitely (famously freezing the NASA Mars Pathfinder rover).
  * **Starvation (Indefinite Blocking):** The vulnerability where a continuous stream of short or high-priority tasks permanently blocks a low-priority job from ever gaining execution time.
* **Open Contemporary Problems & Cyber Horizons:**
  * **Asymmetric Multicore Optimization:** Optimizing real-time scheduling choices for processors that mix radically different compute cores (e.g., Apple M-series performance vs. efficiency cores) without creating severe system bottlenecks or burning out battery systems.
  * **Scheduler Side-Channel Mitigation:** Defending cloud environments against cache-timing exploits (like Spectre variants) where malicious guest VMs analyze CPU scheduling frequencies to steal secret data passing through a shared server rack.

---

### 👑 KEY FIGURES & PREMIER VENUES
* **Important Pioneers:**
  * **Fernando J. Corbató:** Pioneered the Multi-Level Feedback Queue scheduling design within the Compatible Time-Sharing System (CTSS), earning a Turing Award for enabling modern multi-user computing.
  * **Con Kolivas:** Developed the Rotating Staircase DeadLine scheduler for Linux, fundamentally challenging mainstream scheduling philosophies and forcing the creation of modern fair schedulers.
* **Important Venues (Conferences & Journals):**
  * *SOSP (Symposium on Operating Systems Principles):* The world's top research forum tracking elite performance scheduling breakthroughs.
  * *IEEE Transactions on Parallel and Distributed Systems:* The premier archival journal exploring multi-core and cluster resource scheduling mechanics.

---

### 🌐 THE DOMAIN DIMENSIONS
* **Global Perspective:** CPU scheduling algorithms govern the power and efficiency grid of the global internet infrastructure. Even a 0.5% optimization in how cloud servers schedule multi-tenant workloads results in millions of dollars saved in electricity and server hardware across hyperscale datacenters.
* **Local Perspective (CS @ UVT):** Schedulers represent an active programming challenge at the **West University of Timișoara**.
  * Students manually simulate and code classic scheduling models (FCFS, SJF, Round Robin) inside the **Operating Systems labs** to visualize CPU utilization bottlenecks and task starvation thresholds.

---

## 🌲 SYSTEM INTERFACE SELECTOR

> [!NOTE] Architecture Leaf Node
> "This leaf marks the deepest conceptual layer for CPU Scheduling. Navigate back to parent nodes to explore other sub-systems."

* Return to: [[Kernel & Process Management]]
* Return to: [[Operating Systems]]

---