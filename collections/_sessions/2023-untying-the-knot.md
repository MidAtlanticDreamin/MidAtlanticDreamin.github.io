---
title: "Untying the knot: Enabling reflection and decoupling dependencies in Apex"
speakers:
 - "Jonathan Devlin"
layout: session
location: "Main Downstairs"
time: "3 — 3:45pm"
order: "F1"
edition: "2023"
---

The largest roadblock to Apex development in large, enterprise orgs is the hard dependency chain that builds over time on objects and other apex classes. With a few key strategies, those dependencies can be shifted from tightly coupled to loosely coupled. There are two main strategies for this. The first is to use the Callable interface everywhere you have logic of any kind, combined with dynamic type instantiation via a factory. This enables easy mocking/stubbing of other class dependencies, as well as reflection in Apex. The second method is to leverage an Apex object for your classes to operate on rather than directly in on sobject. This allows for decoupling of dependencies on the actual sobjects to exist. Both of these strategies have been wrapped together and enhanced with a few other enterprise patterns (such as unit of work) with the upcoming open source zero dependencies framework from my firm, Booz Allen Hamilton. With this framework, it’s possible to take any apex class built on the framework in the org and deploy only itself + its test class to a fresh scratch org and work on it before merging back to a shared environment. This allows developers to carve out a small piece of functionality and safely work on it in an isolated environment rather than having to share a sandbox with other developers and potentially step on each others toes. Finally, these strategies can be slowly implemented piece by piece, rather than the “all-or-none” approach most frameworks/techniques take.
