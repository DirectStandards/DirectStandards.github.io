---
title: TIM+ Reference Implementation
---

## Overview

The reference implementation is an open source implementation of the TIM+ specification.  The implementation is written in Java using a highly modified version of the Openfire XMPP server.  As with the DirectProject, the reference implementation comes with a standard deployment model to get a TIM+ implementatoin of the ground and running, however it does not meet the requirements of an industry-class production system, such as high availability, failover, scalability and disaster recovery.  It is also for the most part agnostic of policy other than those explicitly outline in the TIM+ specification.  For a TIM+ implementation to become fully compliant with industry best practices, certificate policies and required operational procedures, investment in infrastructure and some software development is necessary.

## Where To Start

At the time of writing, the reference implementation is fully contained within a monolithic Spring Boot application.  The application contains both the core XMPP server that implements the TIM+ specification as well as configuration web application that include 
* Creating TIM+ domains
* Managing certificate and trust stores
* Creating and managing users
* Limiting operational monitoring

You can download the application from the maven central repository here.  Optionally you can build the reference implmentation from source code using the instruction [here](https://github.com/DirectStandards/timplus-ri-build/blob/master/README.md).  Finally, configuration instruction for running the server application can be found here.