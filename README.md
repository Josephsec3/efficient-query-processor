# Efficient Query Processor using C++

## 🚀 Project Description
This repository contains a high-performance C++ solution designed to handle and process dynamic event-based queries efficiently. The core engine utilizes hashing mechanisms to manage state tracking and lookup operations in $O(1)$ average time complexity.

## 🛠️ Technical Highlights
* **I/O Optimization:** Uses `ios_base::sync_with_stdio(false)` and `cin.tie(nullptr)` to decouple C++ streams from C standard streams, drastically reducing execution time for large inputs.
* **Data Structure:** Implements `std::unordered_map` for key-value pair tracking, ensuring fast access and modifications.
* **Query Logic:** 
  * `Event 1`: Increments the specific element state count by 1.
  * `Event 2`: Increments the specific element state count by 2.
  * `Event 3`: Audits if the element state weight is equal to or greater than 2, outputting `Yes` or `No`.

## 💻 Code Structure
The main logic is self-contained within `main.cpp` and structured as follows:
* Dynamic allocation of event types.
* On-the-fly evaluation without redundant memory overhead.

## 🏃 How to Run
Compile the code using any modern GCC compiler supporting C++11 or higher:
```bash
g++ -O3 main.cpp -o processor
./processor
