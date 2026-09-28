# DStructs

A Java library implementing fundamental data structures from scratch.

DStructs is an educational and lightweight data structures library focused on understanding how common data structures work internally, without relying on Java's built-in collection implementations.

The project is designed to grow over time as new data structures and algorithms are implemented.

## Origins

DStructs is based on a previous data structures project I developed in C, where I implemented several linked data structures from scratch, including:

* Singly Linked List
* Circular Linked List
* Doubly Linked List

The goal of DStructs is to bring those implementations into Java while continuing to explore data structures, algorithms, memory management concepts, and object-oriented design.

The original C implementation can be found here:

**[C Data Structures — Linked Lists](https://github.com/Physanto/TADS-and-DSA/tree/main/LinkedList/ImplementationC)**

DStructs is a new implementation and is not a direct translation of the original C code. The project is being redesigned for Java and will evolve independently as new data structures and features are introduced.

```text
C implementation
      │
      │  Linked List
      │  Circular List
      │  Doubly Linked List
      ▼
   DStructs
      │
      │  Java implementation
      ▼
More data structures
      │
      ├── Stack
      ├── Queue
      ├── Trees
      ├── Heap
      └── Graph
```

## Features

Currently, DStructs is under development.

Planned and implemented structures include:

* [ ] Singly Linked List
* [ ] Doubly Linked List
* [ ] Stack
* [ ] Queue

More data structures will be added progressively.

## Installation

DStructs is built with Maven.

### Maven

Add the following dependency to your `pom.xml`:

```xml
<dependency>
    <groupId>io.github.physanto</groupId>
    <artifactId>dstructs</artifactId>
    <version>0.1.0</version>
</dependency>
```

> **Note:** DStructs is currently under development and may not yet be available on Maven Central. For now, clone the repository and build it locally with Maven.

## Usage

Example using a doubly linked list:

```java
import io.github.physanto.dstructs.list.DoublyLinkedList;

public class Main {

    public static void main(String[] args) {

        DoublyLinkedList<Integer> numbers = new DoublyLinkedList<>();

        numbers.add(10);
        numbers.add(20);
        numbers.add(30);

        System.out.println(numbers);
    }
}
```

The API is designed to provide a simple interface while keeping the underlying implementation understandable.

## Project Structure

```text
DStructs/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── io/github/physanto/dstructs/
│   │   │       ├── list/
│   │   │       ├── stack/
│   │   │       ├── queue/
│   │   │       └── node/
│   │   └── resources/
│   │
│   └── test/
│       └── java/
│
├── pom.xml
├── LICENSE
└── README.md
```

DStructs is not intended to replace Java's standard collection framework. Its main purpose is to provide understandable implementations of fundamental data structures.

## Development

Clone the repository:

```bash
git clone https://github.com/physanto/Dstructs.git
cd Dstructs
```

Build the project with Maven:

```bash
mvn clean install
```

Run the tests:

```bash
mvn test
```

## Contributing

Contributions, suggestions, and improvements are welcome.

If you find a bug or have an idea for a new data structure, feel free to open an issue or submit a pull request.

When contributing a new data structure, please include appropriate tests and documentation.

## License

DStructs is released under the MIT License.

See the [`LICENSE`](LICENSE) file for more information.

## Author

**physanto**

GitHub: https://github.com/physanto

If you use DStructs in your project, consider giving credit to the original project and linking back to this repository.
