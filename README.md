# Explanations for the completed task (README)

The source files for all three tasks are [Asciidoc](https://asciidoc.org/) documents:
- [`task1.adoc`](task1.adoc)
- [`task2.adoc`](task2.adoc)
- [`task3.adoc`](task3.adoc)

The result files are both in `.html` and `.pdf`:

- [`task1.html`](task1.html)
- [`task2.html`](task2.html)
- [`task3.html`](task3.html)

For local viewing of html files, images must be downloaded.

- [`task1.pdf`](task1.pdf)
- [`task2.pdf`](task2.pdf)
- [`task3.pdf`](task3.pdf)

## Building from sources

To build `.html` from sources run:

```sh
asciidoctor -a allow-uri-read -r asciidoctor-diagram task<N>.adoc
```

To build `.pdf` from sources run:

```shc
asciidoctor-pdf -a allow-uri-read -r asciidoctor-diagram task<N>.adoc
```

Prerequisites:

- Install [Asciidoctor](https://docs.asciidoctor.org/asciidoctor/latest/install/)
- Install [Asciidoctor PDF](https://docs.asciidoctor.org/asciidoctor/latest/install/)