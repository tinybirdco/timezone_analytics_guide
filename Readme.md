# No Time; Too Fly

## Overview

This Repo is a companion to the Tinybird Guide https://www.tinybird.co/docs/guides/working-with-time.html

## Contents

It contains a Data Generator for example data suitable for examining Date, Time, and Timezones, and how they interact. The data is for simulated sales events across several stores in different timezones, along with a recorded log of the store hours kept.

Particularly relevant is the 'Chatham Islands' store, which simulates sales data across a DST change so you can use it to test whether your handling of DST is correct.

## Deployment

This workspace is structured as a Tinybird Data Project - essentially a set of files which define a Tinybird workspace as code, if you are familiar with Configuration-as-Code then this will be a familiar concept. You can simply push these definitions to a Tinybird workspace to deploy the Datasources and pipe.

You can deploy the Workspace contained in this Repo by:

1. [Signup](https://tinybird.co/signup) for Tinybird
2. Follow the CLI [Quickstart](https://www.tinybird.co/docs/cli.html#) to setup the CLI
3. Follow the [guide](https://www.tinybird.co/docs/cli.html#data-projects) for deploying a Data Project, but use this Repo instead of the ecommerce example.

You can also import the .ipynb to your favourite Notebook environment to work with the sample data generator and validation functions.