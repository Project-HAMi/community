# ContainerDays Singapore 2026 - HAMi Workshop & Talk

**Date:** October 27, 2026
**Event:** ContainerDays & AI Context Singapore 2026 (first edition in Singapore, October 27-28)
**Venue:** Suntec Singapore Convention & Exhibition Centre

The HAMi community brought one hands-on workshop and one conference talk to the first ContainerDays Singapore, covering GPU sharing and scheduling in Kubernetes and GPU utilization for neoclouds.

## Sessions

### Workshop: From Zero to Shared GPUs - Hands-on GPU Scheduling in Kubernetes with HAMi

- **Time:** Oct 27, 12:30-13:15 SGT, Workshop Room
- **Speakers:** 宋净超 / Jimmy Song (VP of Open Source Ecosystem, Dynamia), Reza Jelveh (Solution Architect, Dynamia)
- **Slides:** [Download PDF](./workshop-gpu-sharing-hands-on-jimmysong-rezajelveh-20261027.pdf)
- **Lab guide:** https://github.com/Project-HAMi/hami-workshop

A hands-on session that goes from an empty cluster to a working GPU-sharing environment. Attendees deploy HAMi on their laptops (with or without a GPU) and trace how the device plugin intercepts GPU requests, allocates vGPU resources and works with the scheduler. The workshop walks through the HAMi architecture and GPU virtualization model, then explores the DRA integration path:

- Deploy HAMi and schedule fractional GPU workloads
- See how binpack, spread and topology-aware scheduling policies change allocation
- Learn how third-party schedulers (KAI Scheduler, Volcano) compose with HAMi's isolation layer

### Talk: 10x Your Neocloud's GPU Utilization with HAMi

- **Time:** Oct 27, 15:05-15:40 SGT
- **Speaker:** Reza Jelveh (Head of Global Market, Dynamia)
- **Slides:** [Download PDF](./10x-neocloud-gpu-utilization-rezajelveh-20261027.pdf)

DRA lets Kubernetes request fine-grained GPUs, but it does not solve utilization on its own: devices still need virtualization and a scheduler that knows how to share them. Hardware-agnostic GPU virtualization provides that layer, pooling NVIDIA, AMD, Ascend and domestic NPUs under one scheduler. The talk covers:

- How vGPU interception enforces memory and compute limits
- How the scheduler places heterogeneous devices
- Where DRA fits in, and where it falls short
- Production lessons from cloud providers running 10,000+ GPUs

A blueprint for turning one GPU server into a GPU cloud, with no vendor pitch.

## Resources

- **Event site:** https://www.containerdays.io/containerdays-singapore-2026/
- **Workshop landing page:** https://project-hami.io/landing/containerdays-singapore
- **Talk landing page:** https://project-hami.io/landing/containerdays-singapore-10x
- **HAMi project:** https://github.com/Project-HAMi/HAMi
- **HAMi workshop:** https://github.com/Project-HAMi/hami-workshop
- **Dynamia:** https://dynamia.ai
