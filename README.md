# Aurora Benchmark

This repository contains code used to benchmark the [Aurora static site generator](https://aurora.jamesg.blog).

## About this Benchmark

This repository contains a dataset of [269,452 posts from Hacker News](https://www.kaggle.com/datasets/hacker-news/hacker-news-posts). All of these posts are contained in a single JSONL file, which can be read by Aurora. This project turns each of those files into a template.

This project contains no template inheritence (i.e. using front matter to inherit a template, or using jinja2 to embed a template).

## Use this Benchmark

First, install Aurora from source:

```
git clone https://github.com/capjamesg/aurora
cd aurora
pip install -e .
```

Then, clone this repository:

```
git clone https://github.com/capjamesg/aurora-hn-benchmark
cd aurora-hn-benchmark
```

Finally, run Aurora with the `time` UNIX command to measure the time it takes to generate the dataset:

```
time aurora build
```

## License

The Aurora code is licensed under CC-0. See the [Hacker News dataset source](https://www.kaggle.com/datasets/hacker-news/hacker-news-posts) for information about the license under which the data is covered.
