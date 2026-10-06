# Go → Backend → Distributed Systems → Cloud/K8s → AI Infrastructure

## Phase 1 — Advanced Go

### Go Core
- [ ] Goroutines
- [ ] Channels
- [ ] Buffered vs unbuffered channels
- [ ] `select`
- [ ] Context & cancellation
- [ ] Mutex / RWMutex
- [ ] Atomic operations
- [ ] WaitGroup
- [ ] Worker pools
- [ ] Fan-in / Fan-out
- [ ] Race conditions
- [ ] Go race detector
- [ ] Generics
- [ ] Interface design
- [ ] Error handling patterns
- [ ] Graceful shutdown

### Go Internals
- [ ] G-M-P scheduler model
- [ ] Goroutine scheduling
- [ ] Stack growth
- [ ] Heap vs stack
- [ ] Escape analysis
- [ ] Memory allocation
- [ ] Garbage Collector
- [ ] `GOGC`
- [ ] `GOMEMLIMIT`
- [ ] `sync.Pool`
- [ ] Reflection internals
- [ ] Slice internals
- [ ] Map internals

### Networking
- [ ] TCP fundamentals
- [ ] HTTP/1.1
- [ ] HTTP/2
- [ ] HTTP/3 overview
- [ ] Keep-alive
- [ ] Connection pooling
- [ ] Timeouts
- [ ] DNS basics
- [ ] TLS basics
- [ ] Go `net/http` internals
- [ ] gRPC
- [ ] Protobuf
- [ ] WebSocket / SSE

### Performance
- [ ] Benchmarking
- [ ] `pprof`
- [ ] CPU profiling
- [ ] Memory profiling
- [ ] Goroutine profiling
- [ ] Flame graphs
- [ ] Allocation optimization
- [ ] Lock contention
- [ ] Load testing with k6 / Vegeta

### Project
- [ ] Build high-throughput Go API
- [ ] Add PostgreSQL
- [ ] Add Redis
- [ ] Add worker pool
- [ ] Add graceful shutdown
- [ ] Add metrics
- [ ] Load test
- [ ] Profile
- [ ] Optimize bottlenecks
- [ ] Document benchmark results

---

# Phase 2 — Database Engineering

## PostgreSQL

### Fundamentals
- [ ] B-Tree indexes
- [ ] Composite indexes
- [ ] Covering indexes
- [ ] Partial indexes
- [ ] GIN / GiST overview
- [ ] Query planner
- [ ] `EXPLAIN`
- [ ] `EXPLAIN ANALYZE`

### Internals
- [ ] MVCC
- [ ] WAL
- [ ] VACUUM
- [ ] Autovacuum
- [ ] Transactions
- [ ] Isolation levels
- [ ] Locks
- [ ] Deadlocks
- [ ] Connection management

### Scaling
- [ ] Connection pooling
- [ ] PgBouncer
- [ ] Read replicas
- [ ] Streaming replication
- [ ] Partitioning
- [ ] Sharding concepts
- [ ] Backup / restore
- [ ] Point-in-time recovery

## Redis
- [ ] Redis data structures
- [ ] TTL
- [ ] Persistence
- [ ] RDB
- [ ] AOF
- [ ] Eviction policies
- [ ] Cache-aside
- [ ] Write-through / write-behind
- [ ] Cache invalidation
- [ ] Cache stampede
- [ ] Hot keys
- [ ] Distributed locks
- [ ] Redis Cluster basics

---

# Phase 3 — Production Backend Patterns

## Reliability
- [ ] Timeout
- [ ] Retry
- [ ] Exponential backoff
- [ ] Jitter
- [ ] Circuit breaker
- [ ] Bulkhead
- [ ] Rate limiting
- [ ] Backpressure
- [ ] Load shedding

## Distributed Transactions
- [ ] Idempotency
- [ ] Idempotency keys
- [ ] Optimistic locking
- [ ] Pessimistic locking
- [ ] Outbox pattern
- [ ] Inbox pattern
- [ ] Saga pattern
- [ ] Compensating transactions
- [ ] CDC concepts

## Project — Order/Payment System
- [ ] Order Service
- [ ] Payment Service
- [ ] Inventory Service
- [ ] PostgreSQL
- [ ] Redis
- [ ] Transactional Outbox
- [ ] Async messaging
- [ ] Idempotent consumers
- [ ] Retry mechanism
- [ ] DLQ
- [ ] Simulate duplicate messages
- [ ] Simulate service crashes
- [ ] Prevent double payment

---

# Phase 4 — Distributed Systems

## Theory
- [ ] CAP theorem
- [ ] PACELC
- [ ] Strong consistency
- [ ] Eventual consistency
- [ ] Linearizability
- [ ] Causal consistency
- [ ] Quorum
- [ ] Replication
- [ ] Partitioning
- [ ] Leader / follower
- [ ] Leader election
- [ ] Failure detection
- [ ] Split brain
- [ ] Logical clocks
- [ ] Lamport clocks
- [ ] Vector clocks
- [ ] Gossip protocols
- [ ] Consistent hashing

## Consensus
- [ ] Consensus problem
- [ ] Raft
- [ ] Leader election
- [ ] Log replication
- [ ] Terms
- [ ] Commit index
- [ ] Network partition scenarios
- [ ] Paxos overview

## Messaging
- [ ] Message queues vs event streams
- [ ] At-most-once
- [ ] At-least-once
- [ ] Exactly-once semantics
- [ ] Ordering guarantees
- [ ] Consumer groups
- [ ] Dead Letter Queue
- [ ] Backpressure

---

# Phase 5 — Kafka / Event-Driven Systems

## Kafka
- [ ] Broker
- [ ] Topic
- [ ] Partition
- [ ] Offset
- [ ] Producer
- [ ] Consumer
- [ ] Consumer groups
- [ ] Partition assignment
- [ ] Rebalancing
- [ ] Replication
- [ ] ISR
- [ ] Producer acknowledgements
- [ ] Idempotent producer
- [ ] Transactions
- [ ] Offset management
- [ ] Retention
- [ ] Compaction
- [ ] Schema evolution
- [ ] Schema Registry

## Design
- [ ] Event-driven architecture
- [ ] Event sourcing
- [ ] CQRS
- [ ] CDC
- [ ] Ordering strategies
- [ ] Poison messages
- [ ] Retry topics
- [ ] DLQ strategy

## Project — Distributed Job Queue
- [ ] Scheduler
- [ ] Workers
- [ ] Job persistence
- [ ] Lease mechanism
- [ ] Heartbeats
- [ ] Retry
- [ ] Exponential backoff
- [ ] DLQ
- [ ] Worker failure detection
- [ ] Idempotency
- [ ] Horizontal scaling
- [ ] Metrics

---

# Phase 6 — Observability & SRE

## Observability
- [ ] Structured logging
- [ ] Metrics
- [ ] Distributed tracing
- [ ] Correlation IDs
- [ ] OpenTelemetry

## Metrics
- [ ] Prometheus
- [ ] Grafana
- [ ] RED method
- [ ] USE method
- [ ] Histograms
- [ ] Percentiles
- [ ] p50 / p95 / p99

## Tracing
- [ ] Trace
- [ ] Span
- [ ] Context propagation
- [ ] Cross-service tracing
- [ ] Trace sampling
- [ ] Tempo / Jaeger

## SRE
- [ ] SLI
- [ ] SLO
- [ ] SLA
- [ ] Error budgets
- [ ] Alerting
- [ ] Incident response
- [ ] Postmortems
- [ ] Capacity planning

## Chaos Testing
- [ ] Kill service
- [ ] Kill worker
- [ ] Database latency
- [ ] Redis outage
- [ ] Kafka outage
- [ ] Network latency
- [ ] Packet loss
- [ ] CPU saturation
- [ ] Memory pressure

---

# Phase 7 — Docker & Linux

## Linux
- [ ] Processes
- [ ] Threads
- [ ] Signals
- [ ] File descriptors
- [ ] Sockets
- [ ] `epoll`
- [ ] namespaces
- [ ] cgroups
- [ ] Linux networking
- [ ] DNS
- [ ] iptables / nftables basics

## Docker
- [ ] Container internals
- [ ] Images / layers
- [ ] Multi-stage builds
- [ ] Networking
- [ ] Volumes
- [ ] Resource limits
- [ ] Container security
- [ ] Image optimization

---

# Phase 8 — Kubernetes

## Core
- [ ] Pod
- [ ] Deployment
- [ ] ReplicaSet
- [ ] Service
- [ ] ConfigMap
- [ ] Secret
- [ ] Namespace
- [ ] Ingress
- [ ] StatefulSet
- [ ] DaemonSet
- [ ] Job / CronJob

## Production
- [ ] Requests / Limits
- [ ] Liveness probes
- [ ] Readiness probes
- [ ] Startup probes
- [ ] HPA
- [ ] VPA concepts
- [ ] PDB
- [ ] Rolling deployments
- [ ] Rollbacks
- [ ] RBAC
- [ ] Network Policies
- [ ] Persistent Volumes
- [ ] Storage Classes

## Internals
- [ ] API Server
- [ ] etcd
- [ ] Scheduler
- [ ] Controller Manager
- [ ] kubelet
- [ ] kube-proxy
- [ ] CNI
- [ ] CSI
- [ ] Kubernetes scheduling

## Ecosystem
- [ ] Helm
- [ ] ArgoCD
- [ ] GitOps
- [ ] cert-manager
- [ ] External Secrets
- [ ] Prometheus Operator

---

# Phase 9 — AWS / Cloud

## Networking
- [ ] VPC
- [ ] Public/private subnets
- [ ] Route tables
- [ ] Internet Gateway
- [ ] NAT Gateway
- [ ] Security Groups
- [ ] NACL
- [ ] Route53
- [ ] ALB
- [ ] NLB

## Compute
- [ ] EC2
- [ ] Auto Scaling Groups
- [ ] ECS overview
- [ ] EKS

## Data
- [ ] S3
- [ ] RDS PostgreSQL
- [ ] ElastiCache
- [ ] MSK
- [ ] SQS
- [ ] SNS

## Security
- [ ] IAM
- [ ] IAM Roles
- [ ] Policies
- [ ] KMS
- [ ] Secrets Manager

## Infrastructure as Code
- [ ] Terraform
- [ ] Modules
- [ ] Remote state
- [ ] State locking
- [ ] Environment separation

## Project
- [ ] Provision VPC with Terraform
- [ ] Provision EKS
- [ ] Deploy backend system
- [ ] Deploy PostgreSQL/RDS
- [ ] Deploy Redis
- [ ] Deploy Kafka/MSK
- [ ] Configure ingress
- [ ] Configure autoscaling
- [ ] Add observability
- [ ] Configure CI/CD
- [ ] Configure GitOps
- [ ] Test rollback

---

# Phase 10 — AI/LLM Fundamentals

## LLM Basics
- [ ] Tokens / tokenization
- [ ] Embeddings
- [ ] Transformer architecture
- [ ] Attention
- [ ] Context windows
- [ ] Prompt caching
- [ ] Structured outputs
- [ ] Tool/function calling

## Inference
- [ ] Prefill vs decode
- [ ] KV cache
- [ ] Batching
- [ ] Continuous batching
- [ ] Quantization
- [ ] GPU memory basics
- [ ] Throughput vs latency
- [ ] Time to First Token
- [ ] Tokens/sec

## Python
- [ ] Python sufficient for ML ecosystem
- [ ] NumPy basics
- [ ] PyTorch basics
- [ ] Hugging Face basics
- [ ] Async Python basics

---

# Phase 11 — AI Infrastructure

## LLM Gateway
- [ ] Multi-provider routing
- [ ] Model routing
- [ ] Streaming
- [ ] Retries
- [ ] Fallbacks
- [ ] Rate limiting
- [ ] Quotas
- [ ] Token accounting
- [ ] Cost tracking
- [ ] Request tracing
- [ ] Semantic caching

## Model Serving
- [ ] vLLM
- [ ] Triton Inference Server
- [ ] Hugging Face serving ecosystem
- [ ] Model loading
- [ ] GPU scheduling
- [ ] Model replicas
- [ ] Autoscaling
- [ ] Dynamic batching

## Kubernetes + GPU
- [ ] NVIDIA device plugin
- [ ] GPU requests/limits
- [ ] GPU node pools
- [ ] Node selectors
- [ ] Taints / tolerations
- [ ] GPU autoscaling
- [ ] GPU utilization monitoring

## Project — LLM Gateway
- [ ] Go API gateway
- [ ] Multiple LLM providers
- [ ] Streaming
- [ ] Model fallback
- [ ] Rate limiting
- [ ] Usage tracking
- [ ] Cost tracking
- [ ] Redis caching
- [ ] OpenTelemetry
- [ ] Prometheus metrics
- [ ] Deploy on Kubernetes

---

# Phase 12 — RAG & Search Infrastructure

## Search
- [ ] Information retrieval fundamentals
- [ ] Inverted indexes
- [ ] BM25
- [ ] Dense retrieval
- [ ] Sparse retrieval
- [ ] Hybrid search
- [ ] Reranking

## Vector Search
- [ ] Vector embeddings
- [ ] Cosine similarity
- [ ] Dot product
- [ ] ANN
- [ ] HNSW
- [ ] IVF concepts
- [ ] Vector indexing
- [ ] Metadata filtering

## RAG
- [ ] Document parsing
- [ ] Chunking
- [ ] Embedding pipelines
- [ ] Retrieval
- [ ] Reranking
- [ ] Context construction
- [ ] Query rewriting
- [ ] Hybrid retrieval
- [ ] RAG evaluation
- [ ] Retrieval metrics

## Production
- [ ] Async ingestion
- [ ] Incremental indexing
- [ ] Reindexing
- [ ] Embedding versioning
- [ ] Data isolation
- [ ] Multi-tenancy
- [ ] Caching
- [ ] Observability

---

# Phase 13 — Capstone: AI Platform

## API Platform
- [ ] Authentication
- [ ] API keys
- [ ] Multi-tenancy
- [ ] RBAC
- [ ] Rate limits
- [ ] Quotas

## AI Gateway
- [ ] Multiple providers
- [ ] Self-hosted models
- [ ] Routing
- [ ] Fallback
- [ ] Streaming
- [ ] Load balancing

## RAG Platform
- [ ] Document ingestion
- [ ] Object storage
- [ ] Chunking workers
- [ ] Embedding workers
- [ ] Vector index
- [ ] Hybrid search
- [ ] Reranker
- [ ] Retrieval evaluation

## Async Platform
- [ ] Kafka
- [ ] Worker system
- [ ] Retry
- [ ] DLQ
- [ ] Idempotency
- [ ] Backpressure

## Data
- [ ] PostgreSQL
- [ ] Redis
- [ ] Vector database
- [ ] S3

## Observability
- [ ] OpenTelemetry
- [ ] Prometheus
- [ ] Grafana
- [ ] Distributed tracing
- [ ] LLM latency
- [ ] Token usage
- [ ] Cost/request
- [ ] GPU utilization

## Infrastructure
- [ ] Docker
- [ ] Kubernetes
- [ ] Terraform
- [ ] AWS
- [ ] CI/CD
- [ ] GitOps
- [ ] Autoscaling

## Reliability
- [ ] SLOs
- [ ] Load testing
- [ ] Chaos testing
- [ ] Failure recovery
- [ ] Graceful degradation
- [ ] Disaster recovery

---

# Final Engineering Checklist

## Go
- [ ] Can debug concurrency issues
- [ ] Can profile CPU/memory
- [ ] Understand Go runtime basics
- [ ] Can build high-throughput services

## Backend
- [ ] Can design idempotent APIs
- [ ] Can design async workflows
- [ ] Can diagnose DB performance
- [ ] Can handle partial failures

## Distributed Systems
- [ ] Understand consistency tradeoffs
- [ ] Understand replication
- [ ] Understand partitioning
- [ ] Understand consensus
- [ ] Can reason about failure scenarios

## Production
- [ ] Can investigate p99 latency
- [ ] Can trace requests across services
- [ ] Can define useful SLOs
- [ ] Can handle incidents

## Cloud
- [ ] Can design AWS architecture
- [ ] Can provision using Terraform
- [ ] Can operate Kubernetes
- [ ] Can design CI/CD + GitOps

## AI Infrastructure
- [ ] Understand LLM inference
- [ ] Can build an LLM gateway
- [ ] Can operate model serving
- [ ] Understand GPU workloads
- [ ] Can build production RAG
- [ ] Can measure AI cost/performance

# Target

- [ ] Senior Backend Engineer
- [ ] Distributed Systems Engineer
- [ ] Platform Engineer
- [ ] AI Infrastructure Engineer
- [ ] AI Platform Engineer

**Main path:**

`Go → Backend Internals → Distributed Systems → Kafka → Observability → Linux/Docker → Kubernetes → AWS/Terraform → LLM Systems → AI Infrastructure → RAG/Search → AI Platform`
