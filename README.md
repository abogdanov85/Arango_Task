# Explanations for the completed task (README)

The source files for three tasks are [Asciidoc](https://asciidoc.org/) documents:
- [`task1.adoc`](task1.adoc)
- [`task2.adoc`](task2.adoc)
- [`task3.adoc`](task3.adoc)

Previewing `.adoc` files on GitHub does not work properly, as they do not support `include` statements, diagrams and some other Asciidoc objects.

The result files (built from these sources) are both in `.html` and `.pdf`.

## Results in `.html`

- [`task1.html`](task1.html)
- [`task2.html`](task2.html)
- [`task3.html`](task3.html)

For local viewing of `.html` files, images must be downloaded. 
The images in this repo are the result of building diagrams from text format (`graphviz`). 
So you can either download them together with `.html` or build `.html` locally from sources (see [below](#building-from-sources)).

## Results in `.pdf`

- [`task1.pdf`](task1.pdf)
- [`task2.pdf`](task2.pdf)
- [`task3.pdf`](task3.pdf)

## Building from sources

For building results from sources locally clone this repo:

```sh
git clone https://github.com/abogdanov85/Arango_Task.git
cd Arango_Task
```

For `.html` run:

```sh
asciidoctor -a allow-uri-read -r asciidoctor-diagram task<N>.adoc
```

For `.pdf` run:

```sh
asciidoctor-pdf -a allow-uri-read -r asciidoctor-diagram task<N>.adoc
```

Prerequisites:

- Install [Asciidoctor](https://docs.asciidoctor.org/asciidoctor/latest/install/)
- Install [Asciidoctor PDF](https://docs.asciidoctor.org/asciidoctor/latest/install/)
- Install [Asciidoctor Diagram](https://docs.asciidoctor.org/diagram-extension/latest/installation/)