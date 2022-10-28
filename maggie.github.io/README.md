# American Heart Association - Internal Database Developer Guide

This repository holds the Jupyter Book source for the AHA Internal Database Developer Guide. Only AHA members should have access to the documentation.

1. How to make changes

2. How to build book locally

Table of Contents

1. Introduction
    1. Contributing Members
    2. Database Overview & Current Registries

2. Getting Started with Database
    1. Local Development & Environment setting
    2. Remote Server Setup

3. General Coding Practices and Workflow
    1. GitHub Workflow (Issue, Assigning)
    2. Django Commands with Database Configurations
        Import and Export From Database

# Re-build Jupyter Book 
Tutorials: {https://jupyterbook.org/en/stable/start/overview.html}

Jupyter Book is an open source project for building AHA Database Developer Guild on AHA registry Database from source material that contains computational content.

#### Install Jupyter Book
pip install -U jupyter-book

#### Add new content
Simply add a new .md file in a chapter or open a new chapter if would like in the 'content' folder and write materials.

#### Update Jupyter Book
Once you’ve added content and configured your book, it’s time to build outputs for your book. We’ll use the jupyter-book build command line tool for this. If you add a new file in the _toc.yml file, you can re-run the build command:  

$ jupyter-book build mybookname
