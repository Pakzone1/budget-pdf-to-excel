# Budget PDF-to-Excel API

**Turn budget PDFs into structured spreadsheet output.**

## The problem

The numbers are available. They are just inside a PDF, which is a rather unhelpful place when the next task is spreadsheet analysis.

This service automates the step between receiving a budget document and having structured data in Excel.

## The solution

A FastAPI document-processing service that accepts a PDF, sends it through an AI extraction workflow, converts the structured result into an Excel workbook, and returns the generated file.

## What it does

- PDF upload and processing endpoint.
- AI-assisted extraction into structured data.
- Excel workbook generation with openpyxl.
- Generated output filenames and downloadable results.
- A companion script for processing multiple PDFs.

## Engineering highlights

The pipeline separates document interpretation from workbook creation: PDF -> structured result -> Excel. That boundary makes the output usable by ordinary spreadsheet workflows instead of leaving it as a prose answer in a chat window.

## Technology

Python, FastAPI, OpenAI integration, openpyxl, HTTPX.

## Source code

This repository documents the project, its capabilities, and the engineering behind it. The application source code is maintained privately.
