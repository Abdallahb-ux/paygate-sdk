## Introduction

This project contains a few parts which can be used seperately or in combination, to aid with integration to the payment provider PayGate (https://www.paygate.co.za).

The main components are:

- Standalone Typescript/Javascript client to interface with the PayGate API, usable in any Typescript or NodeJS project
- ExpressJS middleware which can be used to easily configure endpoints for payment processing
- A utility which can help with common PayGate tasks, such as generating payload checksum easily, or extracting a friendly transaction summary message from a payment status response
- Browser script of the utility functions, allowing them to be imported via a `<script>` tag straight into HTML

These components can be used in isolation, or in combination, so you only have to pick what you need in order to help with your specific integration requirements. For example, if you are already using ExpressJS and want to easily enable endpoints that can handle payment processing, then it's likely that the only thing you need from this project is the ExpressJS middleware functions. Or perhaps you want to use the TS/JS client in a Node based project so that you don't have to deal directly with the PayGate HTTP API.

Currently this project is in development, but already quite usable. Reference documentation (currently a work in progress) can be found at https://distributhor.github.io/paygate-sdk/, and more detailed usage info will be made available in this README shortly.