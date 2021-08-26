# A Serverless Runtime on the BEAM

## Introduction

Serverless runtimes are often hidden in a cloud providers offering and exposed solely by their programming API and
deployment procedures. In this blog post, we'll explore an open-source Serverless runtime built for the cloud and
on-premises, running on the BEAM with a polyglot programming model to build general purpose applications.

Building general purpose applications using multiple languages and having a story how to handle state was our main
motivation to explore the space of a Serverless runtime to be built. An open source project, currently hibernating,
based on Akka with a promising technical concept let us to build that runtime. We think the BEAM, OTP and Elixir/Erlang
are a perfect match for that to build on it.

With this blog-post, we combine herein the world of the BEAM with cloud technology like a gRPC-based protocol,
Kubernetes and a polyglot programming model with languages supported like Go, JavaScript, JVM-languages, Python and many
more.
