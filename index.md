---
layout: default
title: "RoboSandbox"
description: "An Open-Source Python Framework for Manipulator Design and Analysis"
---

<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>


![Cover Image](images/callout.svg)

# Supplementary Materials (Anonymous)

This website contains the code and supplementary materials for the RA-L paper.

## Contents

- [Installation](#1)
- [Code](#2)
  - [Code of Use Case A](#3)
  - [Code of Use Case B](#4)

<a id="1"></a>
## Installation

> This section provides instructions on how to install RoboSandbox and verify the installation.


It is recommended to use a virtual environment. To set up a [conda](https://docs.conda.io/en/latest/) and [uv](https://docs.astral.sh/uv/getting-started/installation/) environment with RoboSandbox installed, you can use the following commands:

```bash
conda create -n rsb_env python=3.10
conda activate rsb_env
pip install uv
uv pip install robosandbox
```

To verify the installation, we can launch the app from RoboSandbox:

```bash
python -c "import robosandbox as rsb; rsb.visualization.RobotArmDesignAppStandalone().run_app()"
```

<img src="docs/app.gif" width="800">

<a id="2"></a>
## Code

> This section provides links to the code and showcases the results of the paper.

<a id="3"></a>
### Use Case A

- [Code of Use Case A](docs/use_case_A.html)

- [Part of Plotted Robots](docs/plot_robots.html)

<a id="4"></a>
### Use Case B

- [Optimization of P1](docs/optimization_p1.html)

Code-enriched literature of optimization problem P1:

$$
\min_{\mathbf{a}, \mathbf{d}}\quad f_{1}(\mathbf{a}, \mathbf{d}; \boldsymbol{\alpha^0}) = \delta
$$

- [Optimization of P2](docs/optimization_p2.html)

Code-enriched literature of optimization problem P2:

$$
\min_{\mathbf{a}, \mathbf{d}}\quad f_{2}(\mathbf{a}, \mathbf{d}; \boldsymbol{\alpha^0}) = \delta - G_{n}
$$

- [P1 RRT](docs/example_rrt_p1.html)

Example of robot P1 reaching a target using RRT.

![RRT P1](images/rrt_p1.gif)

- [P2 RRT](docs/example_rrt_p2.html)

Example of robot P2 reaching a target using RRT.

![RRT P2](images/rrt_p2.gif)

- [UR5 RRT](docs/example_rrt_ur5.html)

Example of UR5 reaching a target using RRT.

![RRT UR5](images/rrt_ur5.gif)


- [Compare Gₙ and δ](docs/table_iv.html)
Python script to generate Table IV in the paper.

- [Compare RRT Performance](docs/table_v.html)
Python script to generate Table V in the paper.
