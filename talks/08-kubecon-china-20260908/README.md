# KubeCon China 2026 - HAMi Community Sessions

**Date:** September 8, 2026
**Event:** KubeCon + CloudNativeCon + OpenInfra Summit + PyTorch Conference China 2026, Shanghai
**Venue:** Shanghai International Convention Center
**Booth:** T-1 (Grand Ballroom I)

HAMi's first KubeCon China appearance as a CNCF Incubating project (since July 2026). The community presented **2 keynotes, 1 lightning talk, and 1 conference session**, plus a project booth staffed by maintainers.

## Sessions

### Keynote 1 Operating Frontier Intelligence at Scale

- **Time:** Sep 8, 09:12-09:22, Grand Ballroom II + III
- **Speakers:** Chris Aniszczyk (CTO, Cloud and Infrastructure, The Linux Foundation), 张潇 / Xiao Zhang (Co-founder & CEO, Dynamia)
- **Slides:** [Download PDF](./keynote-operating-frontier-intelligence-at-scale-aniszczyk-zhangxiao-20260908.pdf)

As models are built and AI moves to production, the challenge shifts to making every GPU count: scaling on demand, staying reliable, and understanding increasingly complex systems. Cloud native technology is becoming the OS layer for AI infrastructure. The keynote also covers the growing role of observability and why next-generation AI infrastructure depends on open technologies working together across the stack.

### Keynote 2 PD Disaggregation vLLM Deployment on Alternative AI Accelerators Using llm-d

- **Time:** Sep 8, 09:59-10:04, Grand Ballroom II + III
- **Speakers:** 王纪飞 / Jifei Wang (HAMi Approver, Dynamia), 李孟轩 / Mengxuan Li (Co-founder & CTO, Dynamia)
- **Slides:** [Download PDF](./keynote-pd-disaggregation-vllm-llm-d-wangjifei-limengxuan-20260908.pdf)

llm-d is a CNCF project for distributed LLM inference on Kubernetes. How does PD (Prefill/Decode) disaggregation deploy vLLM efficiently when the inference cluster is no longer NVIDIA-only? This keynote presents llm-d's support for heterogeneous accelerators: HAMi brings heterogeneous GPU sharing and scheduling into llm-d's inference topology, so partitioning, sharing, and scheduling work across hardware architectures.

### Lightning Talk: From Static Slices to Elastic GPUs - Dynamic MIG with HAMi

- **Time:** Sep 8, 11:14-11:19, Room 5B + C
- **Speaker:** 王纪飞 / Jifei Wang (HAMi Approver, Dynamia)
- **Slides:** [Download PDF](./dynamic-mig-with-hami-lightning-wangjifei-20260908.pdf)

NVIDIA MIG on Kubernetes normally requires static pre-partitioning: operators must decide the partition layout before workloads arrive. Too few slices waste the card; too many cause fragmentation. This talk presents a scheduling-driven approach: HAMi integrates the scheduler with the device plugin so GPU partitions follow real-time scheduling decisions — schedule first, partition second, not the other way around.

> GPU partitioning should follow scheduling, not precede it.

### Session: How Intsig Serves Billions of Document Scans - GPU Virtualization at Scale with HAMi

- **Time:** Sep 8, 14:30-15:00, Grand Ballroom II + III
- **Speakers:** 李孟轩 / Mengxuan Li (Co-founder & CTO, Dynamia), Walter Duan (Intsig)
- **Slides:** [Download PDF](./intsig-gpu-virtualization-at-scale-limengxuan-walterduan-20260908.pdf)

A production lesson at ~1000-GPU scale. Intsig (CamScanner, 300M+ downloads worldwide) runs an extreme GPU workload: a single OCR workload, very high concurrency — where the bottleneck is queueing time, not placement. The speakers share the migration from Tencent QGPU to HAMi for one-stop virtualization, scheduling, and monitoring, plus HAMi production case data:

- **SF Express (顺丰):** GPUs reduced from 1,400 to 1,000 with no business impact
- **China Merchants Bank (招商银行):** 10,000+ GPUs, utilization 20% → 80%
- **NIO (蔚来):** 10x CI efficiency improvement
- **ICBC (工商银行):** GPU utilization 20% → 70%

The talk also covers costly anti-patterns (e.g., GPU slices below 1/6 backfire) and a live demo of Chaterm, Intsig's open-source AI terminal for operating GPU clusters in natural language.

## Resources

- **Event site:** https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/
- **Full schedule:** https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/
- **Announcement (中文):** [活动预告｜9 月 8 日，上海见：HAMi 社区亮相 KubeCon China 2026](https://mp.weixin.qq.com/s/msqEpR182YLaUeSn-dCTeg)
- **HAMi project:** https://github.com/Project-HAMi/HAMi
- **llm-d:** https://github.com/llm-d/llm-d
- **Dynamia (密瓜智能):** https://dynamia.ai
- **Intsig (合合信息):** https://www.intsig.com
