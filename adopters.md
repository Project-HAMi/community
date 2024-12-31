# Adopters of HAMi

Below are the adopters of project HAMi. If you are using HAMi to provide device virtualization for several heterogeneous devices including GPU/NPU/MLU, etc,
please feel free to add yourself into the following list by a pull request. There're several phases as follow:

* **Evaluation:** Known HAMi, that's interesting; evaluating the features/scopes of HAMi
* **Testing:** Take HAMi as one of candidates, testing Kubernetes cluster with HAMi
* **Staging:** Decide to use HAMi, testing it in pre-product environment
* **Production:** Already put HAMi into product environment

> Note: If some environment labels are inaccurate, please correct them.



| Organization | Contact | Environment | Description of Use |
|---|---|---|---|
| [4paradigm](http://4paradigm.com/) |[@archlitchi](https://github.com/archlitchi) | Production | device-sharing for third-party devices like (GPU,NPU,MLU),etc. |
| [Linklogis](https://www.linklogis.com/) | [@rnyrnyrny](https://github.com/rnyrnyrny) | Production | Online inference service. |
| [PingAn Securities](https://stock.pingan.com/) | [@detongz](https://github.com/detongz) | Testing/Staging | Used with kubeflow to allocate a single gpu to multiple notebooks, improving work efficiency; occasionally encountered jupyter kernel crashes (later resolved by adjusting parameters). |
| Caper | [@summerisc](https://github.com/summerisc) | Production | Physical gpu partitioning, used with volcano scheduler for automatic training pipelines. |
| [Huawei](https://www.huawei.com/cn/) | [@AlexPei](https://github.com/AlexPei) | Evaluation | Testing resource isolation for multiple deep learning inference services (multi-container) sharing a single card; found that with continuously increasing concurrent requests, video memory continues to increase and does not release after stopping the stress test; the utilization rate of gpu computing units exceeds the set value. |
| [PingAn Bank](https://bank.pingan.com/) | [@jamie-liu](https://github.com/jamie-liu) | Testing | Solved the problem of insufficient gpu resources and improved resource utilization. |
| [Strongit](http://www.strongit.com.cn/) | [@eadou](https://github.com/eadou) | Testing | Used for testing and training ai algorithms. |
| [Beijing Chenan](http://www.gsafety.com/) | [@Chenyangzh](https://github.com/Chenyangzh) | Production | Deep learning algorithm inference. |
| Sinochem Modern Agriculture | [@mazhaoshuo](https://github.com/mazhaoshuo) | Production | Inference. |
| [XW Bank](https://www.xwbank.com/) | [@JJwangbilin](https://github.com/JJwangbilin) | Testing | Solved the problem of gpu computing power isolation. |
| Haofang | [@khw934](https://github.com/khw934) | Evaluation | Testing various gpu virtualization scenarios to fully utilize gpu resources; requested support for using cpu resources to replace gpu computing power; requested support for the function of consolidating fragmented resources (e.g., if one card has 0.3 remaining and another has 0.5, it should be possible to apply for 0.7). |
| R3 | [@Danniez](https://github.com/Danniez) | Production | Infrastructure deployment. |
| [China Mobile](http://www.10086.cn/) | [@ssslkj123](https://github.com/ssslkj123) | Staging/Production | Gpu resource pooling, tenant isolation based on gpu time slicing and memory quota control, machine learning operations, and sales scenarios; offline deployment of helm templates is not user-friendly and deployment is complex. |
| [H3C](https://www.h3c.com/cn/) | [@chenxj1997](https://github.com/chenxj1997) | Testing | Implemented gpu isolation. |
| [Chengqi Technology](http://www.chaintech.com.tw/) | [@x1y2z3456](https://github.com/x1y2z3456) | Testing | Effective gpu isolation. |
| A certain Shenzhen public institution | [@NoKnowKonwNo](https://github.com/NoKnowKonwNo) | Testing | Helm deployment successful; the vgpu-scheduler single pod can only apply for gpu units less than or equal to the number of graphics cards. |
| [Xuanyuan Network Technology Co., Ltd.](https://www.xuanyuan.com.cn/) | [@15220036003](https://github.com/15220036003) | Evaluation/Testing | Using a physical gpu card for teaching, virtualizing multiple vgpus for multiple students; the vgpu-device-plugin plugin could not be installed (later resolved with community help). |
| [Toodata](https://www.i-tudou.com/) | [@51qzpw](https://github.com/51qzpw) | Evaluation | Model inference, image interpretation, and other scenarios. |
| [Infervision](https://www.infervision.com/) | [@freemanke](https://github.com/freemanke) | Evaluation | Model inference. |
| [China East Telecom](http://www.caih.com/) | [@fangfenghuang](https://github.com/fangfenghuang) | Testing | Gpu virtualization to solve gpu resource sharing problems. |
| A certain Chinese enterprise | [@18735100708](https://github.com/18735100708) | Production | Deep learning inference. |
| [China Unicom Industrial Internet](http://www.chinaunicom.com.cn/) | [@zqz199](https://github.com/zqz199) | Evaluation/Testing | Attempting to build a systematic platform for ai training and inference that can allocate gpu resources with fine-grained partitioning. |
| [Chengyu Wisdom](https://www.cyintell.com/) | [@x1y2z3456](https://github.com/x1y2z3456) | Production | Deep learning training, educational and research institutions. |
| Anyuan Huixin | [@nice-jiang](https://github.com/nice-jiang) | Staging/Production | In education, research, and internal enterprise r\&d scenarios, vgpu effectively solves the problem of improving gpu resource utilization. |
| [Technical University of Munich](https://www.tum.de/en/) | [@Ajexsen](https://github.com/Ajexsen) | Evaluation | Master's thesis, federated learning test research and development environment. |
| [Southeast University](https://www.seu.edu.cn/) | [@niconical](https://github.com/niconical) | Evaluation | Preliminary research on gpu resource utilization optimization on the arm64 platform on kubernetes. |
| [Hangzhou Lianhui](https://www.hzlh.com/) | [@louyifei8888](https://github.com/louyifei8888), [@xyy1999](https://github.com/xyy1999) | Evaluation/Testing | Gpu usage isolation, research on maximizing gpu resource utilization. |
| [Woqu](http://www.woqu365.com/) | [@zhuziyuan](https://github.com/zhuziyuan) | Evaluation/Testing | Test GPU sharding |
| [Guangdong University of Technology](https://www.gdut.edu.cn/) | [@cccusername](https://github.com/cccusername) | Evaluation/Testing | research on GPU virtualization technology and GPU isolation 
| [Shenzhen Bode Ruijie Health Technology Co., Ltd.](https://ragehealth.cn/) | [@rainbowechoes](https://github.com/rainbowechoes) | Production | Gpu virtualization inference. |
| A certain industrial internet enterprise | [@Dravening](https://github.com/Dravening) | Production | Various gpu computing tasks scheduled based on k8s, gpu virtualization greatly helps improve gpu resource utilization. |
| [ppio/](https://www.ppio.cn/) | [@zeta65](https://github.com/zeta65) | Evaluation | Ai computing to improve resource utilization. |
| Beijing Unit Technology Co., Ltd. | [@jingzhe6414](https://github.com/jingzhe6414) | Production | Ai computing platform, refined resource allocation. |
| [Nankai University - Network Laboratory](https://ndst.nankai.edu.cn/) | [@liudsl](https://github.com/liudsl) | Evaluation | Preliminary research on gpu computing resource allocation and isolation for scheduling algorithm research. |
| [Institute of Information Engineering, Chinese Academy of Sciences](http://www.iie.ac.cn/) | [@Crownor](https://github.com/Crownor) | Production | Research resource integration and management |
| A certain fund | [@hellobiek](https://github.com/hellobiek) | Production | Financial scenarios, intelligent customer service, intelligent search, etc. |
| [Donghua University](https://www.dhu.edu.cn/) | [@kirakiseki](https://github.com/kirakiseki) | Evaluation/Testing | Use this plug-in to run high video memory demand tasks, use k8s to schedule gpu resources, and provide flexible resource allocation support for learning and training scenarios. |
| [China University of Mining and Technology](https://www.cumt.edu.cn/) | [@hyc-yuchen](https://github.com/hyc-yuchen) | Evaluation | Perform gpu virtualization and use k8s to schedule gpu resources. |
| [iFlytek](https://www.iflytek.com/) | [@whybeyoung](https://github.com/whybeyoung) | Production | Public cloud reasoning, training. |
| [Beijing East China Information Technology Co., Ltd.](https://www.bonc.com.cn/) | [@xieyyan](https://github.com/xieyyan) | Production | Ai gpu speed limit. |
| [gsafety](http://www.gsafety.com/)| [@liuchunhui-c](https://github.com/liuchunhui-c) | Production | 3 nodes reasoning training. |
| [Miaoyun](https://www.miaoyun.net.cn/) | [@erganzi](https://github.com/erganzi) | Evaluation | Perform gpu virtualization and use k8s to schedule gpu resources. |
| Chongyue Computer Network Technology Co., Ltd. | [@stormdragongardin](https://github.com/stormdragongardin) | Evaluation/Testing | Cloud platform development. |
| [Guangzhou Pingao](https://www.bingosoft.net/) | [@zhangQiWorr](https://github.com/zhangQiWorr) | Evaluation | Gpu heterogeneous resource scheduling research. |
| [Shanghai Aisha Medical Technology Co., Ltd.](https://www.ashermed.com/) | [@shown1985](https://github.com/shown1985) | Testing | Internal testing. |
| [Kylinsoft](https://www.kylinos.cn/) | [cuiyudong-free](https://github.com/cuiyudong-free) | Testing/Staging | Deploy hami functions in ai scenarios of cloud base operating system/server operating system. |
| [Harbin Institute of Technology](http://www.hit.edu.cn/) | [@blackjack2015](https://github.com/blackjack2015) | Production | Gpu cluster management of the research group. |
| [MSXF](https://www.msxf.com/) | [@xiaoyao](https://github.com/xiaoyao) | Testing | Gpu sharing in development environment, heterogeneous gpu management. |
| [Tongcheng Travel](https://www.ly.com/) | [@devenami](https://github.com/devenami) | Production | Inference service gpu sharing, improve gpu utilization; gpu model: l40s, a800. |