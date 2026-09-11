# HAMi Meetup - Shanghai 2026 (Incubating Special)

**Date:** September 6, 2026
**Location:** Shanghai
**Co-organizers:** Dynamia (密瓜智能) & HAMi Community, with 上海五角场创新创业学院

"不卷算力，卷效率" — the 4th HAMi community meetup and the first offline HAMi event since the project joined CNCF Incubating (July 2026). One opening speech, five technical talks, and a community panel covering remote GPU, distributed inference, domestic GPU adaptation, heterogeneous scheduling, and AI platform engineering.

## Presentations

### Opening: CNCF × PyTorch — Building a Cloud Native AI R&D Foundation

- **Speaker:** Keith Chan - CNCF China Director & Linux Foundation APAC VP
- No slides archived

### From Local Devices to Remote Compute Pools: Remote GPU and HAMi 2.10

- **Speaker:** 李孟轩 - Dynamia 密瓜智能 Co-founder & CTO, HAMi Author & Maintainer
- **Topic:** Remote GPU releasing devices from node boundaries; HAMi v2.10 updates including KAI Scheduler adaptation, vNPU slicing & monitoring, mutex scheduling policies, flexible dynamic MIG, and HAMi-DRA progress on device allocation, resource reuse, and Ascend support
- [Download PDF](./remote-gpu-hami-2.10-limengxuan.pdf)

### llm-d: A Distributed Inference Plane Across Workloads, Modalities, Hardware, and Platforms

- **Speaker:** 张家驹 - Red Hat Greater China CTO
- **Topic:** llm-d as an independent inference control plane — smart routing, KV Cache management, Prefill/Decode disaggregation, flow control, autoscaling, and batch processing; v0.8 direction including EndpointDiscovery extending scheduling beyond Kubernetes to Slurm, bare metal, and RL training
- [Download PDF](./llm-d-distributed-inference-plane-zhangjiaju.pdf)

### High-Performance Inference Deployment on Iluvatar GPUs

- **Speaker:** 叶成林 - 天数智芯 (Iluvatar CoreX) Infra R&D Director
- **Topic:** Full engineering path for domestic GPU inference: IxFormer / IXInfer / ixDNN / ixBLAS / IXCCL / IXLink software stack, unified resource control plane with Device Plugin, DRA, topology scheduling, and HAMi GPU sharing; SLO-driven acceptance from device allocation to First Token (TTFT, TPOT, Scale-to-First-Token, KV Transfer)
- [Download PDF](./iluvatar-gpu-inference-deployment-yechenglin.pdf)

### Building a K8s Heterogeneous AI Compute Base with Volcano + HAMi-core

- **Speaker:** 董江 - 科大讯飞 (iFLYTEK) Senior Architect, Volcano & HAMi Community Member
- **Topic:** Volcano unifying multi-engine orchestration, queue management, DAG workflows, gang scheduling, and bin-pack scheduling (40% utilization gain), combined with HAMi-core for GPU memory/compute isolation and fine-grained slicing
- [Download PDF](./volcano-hami-core-k8s-ai-base-dongjiang.pdf)

### Engineering Challenges and Practices of AI Computing Platforms

- **Speaker:** 彭鹏 - UCloud Senior R&D Engineer
- **Topic:** Five engineering gaps in dev-environment delivery: unified resource expression (Instance Spec), lightweight multi-cluster access, runtime tool injection, on-demand image loading, and scenario-based GPU isolation (HAMi vGPU for private platforms, kernel-level vGPU for public-cloud C-end, QEMU passthrough / NVSwitch fabric trade-offs for B-end)
- [Download PDF](./ucloud-ai-platform-engineering-pengpeng.pdf)

### HAMi Ambassador Program Launch

- **Speaker:** Jimmy Song - Dynamia 密瓜智能 VP of Open Source Ecosystem
- **Topic:** On-site launch of the HAMi Ambassador Program: charter, recognition, and how to join
- [Download PDF](./hami-ambassador-program-launch-jimmysong.pdf)

## Community Panel

The panel discussed the journey from HAMi user to contributor, how AI Coding should enter open source collaboration (contributors must understand and take responsibility for AI-assisted code), and HAMi's next steps toward AI (MCP & automated diagnostics, project knowledge base, mixed model sizes, and growing domestic heterogeneous compute).

## Resources

- **Event recap (中文):** https://dynamia.ai/zh/blog/hami-meetup-shanghai-2026
- **HAMi Ambassador Program:** [../ambassador-program.md](../../ambassador-program.md)
- **HAMi project:** https://github.com/Project-HAMi/HAMi
- **Dynamia (密瓜智能):** https://dynamia.ai
