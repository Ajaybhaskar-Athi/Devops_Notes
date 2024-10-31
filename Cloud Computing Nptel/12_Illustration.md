### Problem: Counting Word Frequencies in a Huge Collection of Documents

Imagine we have an enormous collection of documents, like all the web pages on the internet. Our goal is to find out how often each word appears in this collection. Let’s say we have:
- **n** = the total number of documents
- **m** = the total number of unique words (for which we want to calculate frequencies)

We want to determine the frequency of each unique word in the collection. Since the collection is so large, we need to distribute this work across multiple processors.

---

### **Two Approaches to Count Word Frequencies:**

1. **Divide the words among processors**:  
   - Each processor handles the counting for about **m/p** words (where *p* is the number of processors).
   - This approach allows each processor to focus on a smaller subset of words, reducing the total workload per processor.

2. **Divide the documents among processors**:  
   - Each processor reads **n/p** documents, calculating the word frequencies for *all m words* within its assigned set of documents.
   - Then, all processors combine their counts to get the final word frequency.

---

### **System Model: Parallel Processing with Shared Disk**

- **Distributed-Memory Model with Shared Disk**: Each processor has its own memory but can access a common disk where all documents are stored. 
- **Advantage**: Any processor can access any document without waiting for other processors, allowing them to work in parallel without competition for data access.

---

### **Time Analysis for Processing Words:**

- **Time to read a word from a document** is represented as **c** = - **Time to send a word’s frequency data to another processor** (if needed) is represented as **c**.
- **Time to add to the total frequency count is very small** and is considered negligible.
- Each word appears an average of **`f times`** in each document.

With a single processor:
- **Total time for computing all word frequencies** = `n × m × f × c`=n × m/p × f  where [c=1/p]

---

### **First Approach: Divide Words Among Processors**

- With **p processors**, each one processes about **m/p words**.
- Each processor reads up to `n × (m/p) × f` times from the shared disk.

---
### **Second Approach: Divide Documents Among Processors**

### Second Approach: Counting Word Frequencies with Distributed Document Processing

In this second approach, we assign each processor a subset of **n/p** documents, where:
- **n** is the total number of documents.
- **p** is the total number of processors.
  
Each processor calculates word frequencies for **all m words** within its assigned set of documents, rather than a subset of words, which was the focus of the first approach.

---

### Steps and Time Analysis 

1. **Document Reads by Each Processor**
   - Each processor reads about **`n/p × m × f`** words from its assigned documents.
   



  
4. **Calculating Parallel Efficiency**
   - **Parallel Efficiency** considers the time it would take a single processor to complete the task versus the combined time for all processors. Efficiency generally decreases as **p** increases due to added overhead in communication and synchronization.

# Parallel efficiency is computed as:= 1 / (1+(2p/nf));
