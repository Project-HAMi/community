# KubeCon NA 2026 - HAMi Community Sessions

**Date:** November 9-10, 2026
**Event:** KubeCon + CloudNativeCon North America 2026 (November 9-12), Salt Lake City
**Venue:** Salt Palace Convention Center
**Booth:** CNCF Project Pavilion

HAMi's first KubeCon North America as a CNCF Incubating project. The community presented a joint talk with Red Hat at Cloud Native AI + Inference Day, a Maintainer Track session and an 80-minute ContribFest, plus a project booth.

## Sessions

### Cloud Native AI + Inference Day: DRA + Kueue + HAMi + vLLM/llm-d - A Production Architecture for Scheduler-Agnostic GPU Sharing

- **Time:** Nov 9, 15:20-15:45, Level 2, 251 D-F
- **Speakers:** 李孟轩 / Mengxuan Li (Co-founder & CTO, Dynamia), Yuchen Fama (Senior Principal Product Manager, Red Hat)
- **Slides:** [Download PDF](./inference-day-dra-kueue-hami-llm-d-limengxuan-yuchenfama-20261109.pdf)

Not every inference workload needs a whole GPU: embedders, rerankers, classifiers and speech models keep consuming GPU time too. The talk shows how DRA describes and allocates devices, HAMi handles GPU partitioning and in-container isolation, and Kueue provides quota management and admission control.

GPU sharing alone does not fix inference performance. When vLLM instances each own their KV cache, cache-unaware load balancing scatters same-prefix requests and wastes memory, which hurts more on smaller GPU slices. llm-d's EPP (Endpoint Picker) routes requests to instances that already hold the prefix cache. In an MI355X experiment with three vLLM instances at 30% HBM each and 8 QPS, enabling EPP raised the prefix cache hit rate from 45.2% to 92.4% and cut TTFT P90 from 251 ms to 157 ms.

### Maintainer Track: HAMi Levels up - Smarter Scheduling, Wider Hardware Reach and a DRA-Native Lightweight Future

- **Time:** Nov 10, 14:50-15:20, Level 2, 251 D-F
- **Speaker:** 李孟轩 / Mengxuan Li (HAMi maintainer, Co-founder & CTO, Dynamia)
- **Slides:** [Download PDF](./maintainer-track-hami-levels-up-limengxuan-20261110.pdf)

HAMi's first Maintainer Track session since becoming a CNCF Incubating project, covering the latest progress:

- **Composable scheduling policies:** Mutex, Spread and NUMA-aware placement can be combined
- **Flexible-MIG:** pick a MIG partition template from the Pod's request at scheduling time instead of pre-slicing GPUs
- **Remote-GPU:** apps on CPU-only nodes access GPUs on other nodes over the network
- **AMD:** full support in HAMi v2.10, including GPU partitioning, compute isolation, AMD-DRA and real usage monitoring
- **HAMi-DRA:** a DRA driver that plugs into Kubernetes-native allocation while keeping HAMi's partitioning and isolation

### ContribFest: GPU Virtualization - First Setup and Understanding the Device Plugin / DRA

- **Time:** Nov 10, 16:40-18:00 MST, Level 2, Room 255 D
- **Speakers:** Reza Jelveh (Solution Architect, Dynamia), 李孟轩 / Mengxuan Li (HAMi maintainer, Dynamia), 申涵 / Han Shen (HAMi-WebUI Reviewer, Dynamia)
- **Slides:** [Download PDF](./contribfest-gpu-virtualization-first-setup-rezajelveh-limengxuan-shenhan-20261110.pdf)
- **Schedule:** https://events.linuxfoundation.org/kubecon-cloudnativecon-north-america/program/schedule/?id=1294775

An 80-minute hands-on session that needs only a laptop, no GPU. Attendees install HAMi on kind with mock GPUs (mock-device-plugin and hami-mock-monitor), share GPUs across Pods, compare binpack and spread policies, and trace where topology information comes from. The lab walks through the full Pod path: admission webhook, HAMi scheduler, device plugin `Allocate`, and HAMi-Core enforcement. It then dives into DRA (ResourceSlice, DeviceClass, ResourceClaim, consumable capacity) and HAMi-DRA, which converts HAMi GPU requests into ResourceClaims. Attendees leave with a path to a first contribution to HAMi, HAMi-DRA, the mock device plugin or HAMi WebUI.

## Resources

- **Event site:** https://events.linuxfoundation.org/kubecon-cloudnativecon-north-america/
- **ContribFest landing page:** https://project-hami.io/landing/kubecon-na-contribfest
- **Recap (中文):** [技术演进+动手实践：HAMi 在 KubeCon NA 2026 的回顾](https://mp.weixin.qq.com/s/b0P0E-w9Pg8R49mOYG_wVg)
- **HAMi project:** https://github.com/Project-HAMi/HAMi
- **HAMi-DRA:** https://github.com/Project-HAMi/HAMi-DRA
- **llm-d:** https://github.com/llm-d/llm-d
- **Kueue:** https://github.com/kubernetes-sigs/kueue
- **Dynamia:** https://dynamia.ai
