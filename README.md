# Build a Media Agent: CPU Agent, GPU Models as Tools

Hands-on workshop by Alexey Grigorev — Tuesday, 3 November 2026, 16:30 Berlin time.

In this workshop we build a media agent where a lightweight agent running on a CPU acts as the control plane, and GPU models deployed on Nebius Serverless Endpoints are its tools. The agent calls text-to-image and text-to-speech models through MCP, inspects what comes back, and decides what to do next. Along the way we compare two ways of running the GPU side — an always-on Endpoint and a batch Job — on latency and cost per generated asset.

## Outline

1. **Setup and why: CPU for the agent, GPUs for the models** (10 min)
2. **First tool:** wrap a text-to-image model on a Nebius Serverless Endpoint as `generate_image(spec)`, which returns an Object Storage link (20 min)
3. **CPU agent as the control plane:** take a brief and decide which tools to call, then add text-to-speech as a second tool via MCP (25 min)
4. **Endpoint vs Job:** run the same generation as a batch Job for 50 records and compare latency and cost per asset (20 min)
5. **What's next:** the capstone (Personalized Media Factory), plus Q&A (15 min)

## Prerequisites

- A Nebius account with credits
- [uv](https://docs.astral.sh/uv/) installed

## Code

The code will be published in this repository before the workshop.

## Want to go deeper?

This workshop is a preview of the course **Production AI Agents for Generative Media**: [register here](https://courses.datatalks.club/register/production-ai-agents-generative-media/).
