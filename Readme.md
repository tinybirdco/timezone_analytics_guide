# No Time; Too Fly

## Overview

This repo is a companion to the Tinybird Guide https://www.tinybird.co/docs/guides/working-with-time.html

## Contents

### Tinybird data project

In the [`./tinybird`](./tinybird/) you'll find a Tinybird data project. This contains the Data Sources to ingest data, and the Pipes to query it. The Pipes contain example SQL queries for working with time data.

### Example data generator

The [`./sample_data_generator.ipynb`](./sample_data_generator.ipynb) file can generate data suitable for examining Date, Time, and Timezones, and how they interact. The data is for simulated sales events across several stores in different timezones, along with a recorded log of the store hours kept.

Particularly relevant is the 'Chatham Islands' store, which simulates sales data across a DST change so you can use it to test whether your handling of DST is correct.

## Deployment

First, clone this repo.

You'll then need to deploy the Tinybird data project. To do so:

1. [Signup](https://tinybird.co/signup) for Tinybird
2. Follow the [Quick Start (CLI) guide](https://www.tinybird.co/docs/quick-start-cli.html) to get setup with the Tinybird CLI
3. Enter the `./tinybird` directory
4. Run `tb auth` and authenticate the CLI with your Workspace
5. Run `tb push` to push the data project to Tinybird

You can then use the `./sample_data_generator.ipynb` to generate mock data to your Tinybird Workspace. In the Tinybird UI, you can execute the queries inside the Pipes to learn how to work with Time functions.

You can also import the .ipynb to your favourite Notebook environment to work with the sample data generator and validation functions.

## Read more

1. [Working with Time guide](https://www.tinybird.co/docs/guides/working-with-time.html)
2. [Best practices for Timestamps](https://www.tinybird.co/docs/guides/best-practices-for-timestamps.html)