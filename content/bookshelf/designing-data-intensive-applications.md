---
title: "Designing Data-Intensive Applications"
date: 2025-08-31
draft: false
tags: ["systems", "databases", "distributed-systems", "architecture"]
categories: ["books"]
author: "Martin Kleppmann"
publisher: "O'Reilly Media"
year: "2017"
isbn: "978-1449373320"
pages: "616"
book_url: "https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373320"
reading_status: "read-notes"
rating: "5"
summary: "The definitive guide to understanding the architecture of modern data systems, covering reliability, scalability, and maintainability."
ShowToc: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowShareButtons: true
---

## About This Book

One of the most comprehensive books on data systems architecture. Kleppmann does an excellent job explaining complex distributed systems concepts with real-world examples and trade-offs.

## Key Takeaways

- Data systems are about managing trade-offs between consistency, availability, and partition tolerance
- Understanding the fundamentals is more important than following trends
- Every architectural decision has consequences that compound over time
- Reliability and maintainability should be design goals, not afterthoughts

## My Notes

### Chapter Highlights

**Part I: Foundations of Data Systems**
- Reliability, scalability, and maintainability are the core concerns
- Data models shape how we think about problems
- Storage engines determine performance characteristics

**Part II: Distributed Data**
- Replication strategies and their trade-offs
- Partitioning for scalability
- Transactions in distributed systems

**Part III: Derived Data**
- Batch processing for analytics
- Stream processing for real-time systems
- Building reliable data pipelines

### Important Concepts

- **CAP Theorem**: You can't have all three of consistency, availability, and partition tolerance
- **Two-Phase Commit**: Ensures atomicity in distributed transactions but has availability issues
- **Event Sourcing**: Store events rather than current state for better auditability
- **Lambda Architecture**: Combine batch and stream processing for completeness and low latency

### Actionable Insights

1. Choose boring, well-understood technologies for critical systems
2. Design for failure - assume components will fail
3. Monitor everything, especially distributed system boundaries
4. Keep data formats backward and forward compatible

### Favorite Quotes

> "The major difference between a thing that might go wrong and a thing that cannot possibly go wrong is that when a thing that cannot possibly go wrong goes wrong it usually turns out to be impossible to get at or repair."

## My Review

### What I Liked

- Exceptional depth without getting lost in implementation details
- Real-world examples from major tech companies
- Balanced discussion of trade-offs rather than prescriptive solutions
- Excellent diagrams and visual explanations

### What Could Be Better

- Could use more recent examples (book is from 2017)
- Some chapters are quite dense and might benefit from more code examples

### Who Should Read This

- Software architects and senior engineers
- Anyone building distributed systems
- Database administrators and data engineers
- Technical leaders making infrastructure decisions

### My Rating: 5/5

Essential reading for anyone serious about building data systems. This book has fundamentally changed how I think about data architecture.

## Related Books

- "Building Microservices" by Sam Newman
- "Distributed Systems" by Maarten van Steen
- "Database Internals" by Alex Petrov

## Links

- [📚 Buy on Amazon](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373320)
- [📝 My Detailed Notes](#)