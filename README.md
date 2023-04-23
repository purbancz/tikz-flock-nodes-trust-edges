# TikZ Code Snippet | Flock Nodes with Trust Edges ![build](https://github.com/purbancz/tikz-flock-nodes-trust-edges/actions/workflows/build.yml/badge.svg) ![GitHub](https://img.shields.io/github/license/purbancz/tikz-flock-nodes-trust-edges)


### Table of Contents
- [Introduction](#introduction)
- [Usage](#usage)
- [Motivation](#motivation)
- [License](#license)

## Introduction

This code generates an example of a LaTeX TikZ diagram with five main circular nodes that are irregularly distributed, and each surrounded by a larger group of smaller circular nodes that are unevenly distributed and closer to their respective main node. The edges between the main nodes have varying thickness to represent the strength of the connection between them. Using negative values for the `shorten` option will extend the edges beyond the nodes and eliminate the gap between them to make sure that even the thick edges touch the nodes they connect entirely.
![The diagram consists of five filled circles. Each circle has a random position within a certain range. Around each circle, there are several smaller filled circles that are randomly positioned. The larger circles are connected by lines with varying thicknesses.](/assets/images/tikz_flock.png)

## Usage

The code requires the `tikz` package (with the `calc` library) to be added in the preamble.
```latex
\usepackage{tikz}
\usetikzlibrary{calc}
```
The `tikzpicture` can be easily wrapped with the `figure`  envirement which gives its features of labelling, captioning and float positioning etc.

## Motivation

This diagram is meant to demonstrate the execution of an algorithm that is based on the Evolutionary Multi-Agent System and includes socio-cognitive elements. The population is divided into flocks managed by agents. Each cycle includes an evolutionary part and a socio-cognitive part. During the evolutionary part, agents perform an evolutionary algorithm on their flock. During the socio-cognitive part, agents communicate and exchange information based on trust. The more trust between agents, the more information they exchange. The algorithm continues until a given number of cycles are performed.

On the diagram, the larger nodes stand in for the agents, while the edges symbolize the trust (therefore communication and information exchange) between them and the smaller nodes represent their flocks. Yet, evidentely it can be easily utilized to represent anything of the kind.

## License

This toy-example TikZ snippet is licensed under the MIT license.
___

This is the end of a `README`, you can [click here to go back to the Table of Contents](#table-of-contents).
