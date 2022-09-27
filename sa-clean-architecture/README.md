<h1>Clean Architecture</h1>

<figure>
  <img
  src="docs/clean-architecture-0.svg"
  alt="The beautiful Clean Architecture">
  <figcaption>Figure 1. The clean architecture</figcaption>
</figure>

<h2>Book</h2>
[Clean Architecture by Robert C. Martin](https://www.goodreads.com/book/show/18043011-clean-architecture)

<h2>Concepts</h2>

The diagram in Figure 1 shows that each layer in the Clean Architecture
is responsible for some area of software. The farther inward you go, the
higher level software becomes.

Inner circles are the policies of the software application. The outer
circles are the details of implementation.

Even though the number of circles is four in Figure 1, it's not
fixed and can vary depending on the application.

The Clean Architecture produces the system that is:
<ul>
    <li>Easy to test;</li>
    <li>Independent of frameworks;</li>
    <li>Independent of the UI;</li>
    <li>Database agnostic;</li>
    <li>Independent of any external agency.</li>
</ul>

<h2>The Dependency Rule</h2>

Inner circles must never depend on the outer. However, the flow of
control is going outward. We should use the <b>Dependency Inversion
Principle</b> to resolve such a contradiction.

<h3>Dependency Inversion Principle</h3>

The Dependency Inversion Principle (DIP) states that higher-level
modules should not depend on low-level modules. They should both
depend on abstractions.