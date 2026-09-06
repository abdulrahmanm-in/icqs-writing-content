---
title: "Building FocusSprint: A Full-Stack Task Management App"
description: "How I built FocusSprint with Angular, FastAPI, and PostgreSQL while learning more about authentication, APIs, database design, and full-stack development."
date: "2026-09-06"
category: "Projects"
tags:
  - FocusSprint
  - Angular
  - FastAPI
  - Python
  - PostgreSQL
  - REST API
  - Full Stack
published: true
---

## Why I built FocusSprint

I wanted to build something that would take me beyond simply creating individual frontend or backend features.

I wanted a project where the frontend, backend, database, authentication, and API design all had to work together.

That became **FocusSprint**, a full-stack task management application built with Angular, FastAPI, and PostgreSQL.

The idea itself is simple: give users a place to manage their tasks.

But the interesting part for me wasn't the idea. It was everything involved in building the application behind it.

## The stack

I built FocusSprint using three main technologies:

- **Angular** for the frontend
- **FastAPI** for the backend
- **PostgreSQL** for data storage

The application communicates through a REST API, with authentication handled using JWT tokens.

This gave me an opportunity to work across the full stack instead of focusing on only one layer.

Each layer has a specific responsibility, which helped me understand how the pieces of a real application fit together.

## Authentication was one of the important pieces

One of the things I wanted to implement properly was authentication.

FocusSprint uses JWT-based authentication so that users can securely access their account and the resources associated with it.

The general flow is:

```text
User
 ↓
Login
 ↓
FastAPI validates credentials
 ↓
JWT token
 ↓
Angular handles the authenticated state
 ↓
Token included with protected API requests
```

This was useful because authentication stopped being something I only understood conceptually.

I had to think about how authentication flows through the frontend, how protected endpoints work, and how the backend determines whether a request is allowed to continue.

## Designing the API

The backend exposes more than 15 REST API endpoints covering the application's functionality.

While building them, I started paying more attention to something that is easy to overlook when learning:

**An API isn't just a collection of endpoints.**

The structure of those endpoints, the request and response models, validation, error handling, and authentication all contribute to how usable the API is.

FastAPI made this particularly interesting because request validation and API documentation are closely integrated into the development workflow.

It also made it easy to inspect and test endpoints while developing the application.

## PostgreSQL and database design

FocusSprint uses PostgreSQL as its database.

Working with a real relational database was an important part of the project because I had to think about how application data should actually be stored and related.

Instead of treating the database as something behind the scenes, I started thinking more about:

- What entities does the application need?
- What relationships exist between them?
- Which fields should be required?
- What data should belong to a particular user?
- How should the API interact with the database?

These decisions affect the application much more than they initially appear to.

## Validation and error handling

Another area I focused on was making the API behave predictably when something goes wrong.

Input validation helps prevent invalid data from reaching the business logic, while structured error handling gives the frontend something consistent to work with.

This is one of those areas that isn't particularly exciting to show in a screenshot, but it makes a big difference to the quality of an application.

A successful request is only part of the story.

A good application also needs to know how to handle:

- Invalid input
- Missing data
- Unauthorized requests
- Invalid authentication
- Resources that don't exist
- Unexpected failures

Building these cases into FocusSprint helped me understand backend development beyond simply creating CRUD endpoints.

## What I learned

The biggest lesson from FocusSprint wasn't a particular framework or library.

It was learning how the different parts of an application depend on each other.

A change in the database can affect the backend.

A change in an API response can affect the frontend.

Authentication affects both sides.

Validation affects the API contract.

And a small decision in one part of the application can sometimes have consequences somewhere else.

That made the project much more valuable than simply following a tutorial and reproducing the same application.

## Building it also changed how I think about projects

When I started, I was mostly thinking about getting features to work.

As the project progressed, I started thinking more about how those features should be structured.

There is a difference between:

> "The application works."

and:

> "The application is structured in a way that I can continue working on it."

That distinction is something I'm still learning, but FocusSprint gave me a practical way to experience it.

## What's next

FocusSprint is also part of a larger shift in what I want to work on.

I've been increasingly interested in Python, backend development, APIs, and the systems behind applications.

Building this project gave me a chance to explore those areas through something I could actually use and demonstrate.

There is still plenty I could improve, but that's part of the point.

A project doesn't have to be perfect to be useful.

Sometimes the most valuable projects are the ones that leave you with a better understanding of what you want to learn next.

## Final thoughts

FocusSprint started as a task management project, but it became more of a full-stack learning exercise for me.

I got to work with Angular on the frontend, FastAPI and Python on the backend, PostgreSQL for persistence, JWT authentication, REST APIs, validation, and structured error handling.

More importantly, I got to experience how those pieces come together as one application.

That's what made building FocusSprint worthwhile.
