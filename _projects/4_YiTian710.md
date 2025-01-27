---
layout: page
title: YiTian710
description: Alibaba’s Yitian 710 Is China’s First Homegrown Cloud-Native CPU to Be Put Into Large-Scale Use, 
img: /assets/img/YiTian710.png
importance: 1
category: work
related_publications: false
---

YiTian710 is fabricated in cutting edge 5nm technology. Though YiTian710 only for internal use now and no public benchmarks results available, it still stands for the most powerful ARM Server nowadays with **510 SPEC@2017** Int Rate scores.


<div>
    <img class="three" src="{{ site.baseurl }}/assets/img/ARM_N2_Ref.png" alt="" title="ARM N2 Reference Design"/>
</div>

<div class="three caption">
<strong> ARM N2 Reference Design@ARM.</strong> YiTian710 uses a similar mesh based NoC.
</div>

### Production Spec
[https://apsara-stack.aliyun.com/activity/AlibabaCloudServer_Mseries](https://apsara-stack.aliyun.com/activity/AlibabaCloudServer_Mseries). Sorry, Chinese only.
* 128 ARM v9 core
* Up to 3.0GHz
* TDP 250W
* 8xDDR5 4800MHz
* 96xPCIe Gen5
* Server class RAS features for reliability.
* OpenBMC based server management 

### Mission and Core-Value: 
I was one of the YiTian710 project initial group.
<div>
    <img class="three" src="{{ site.baseurl }}/assets/img/Initial_Team.png" alt="" title="Initial Team"/>
</div>
My mission is to ensure:
1. <strong> High level SoC arhictecture/feature; Ensure final product meets the requirement </strong>
  *  We did it! Commercialized <strong> in one shot. </strong> 
2. <strong> Succeed in one tapeout, No blocking bugs or archiecture defects. </strong>
  *  We did it! Mass Production <strong> in one shot </strong>.
3. <strong> Commercial landing within shortest time  </strong>
  *  We did it! Mass Production <strong> in 12 months </strong> after bringup.

#### I endeavored in following aspect to achieve this goal:
1. <strong> Team Building: </strong> 
    1. Build the entire system software team and software stack from 0
2. <strong> Pre-Silicon: Architecture Ratification & Validation </strong> 
    1. Conduct end to end system level validation to ensure SoC meets the spec.  
3. <strong> Post-Silicon: Chip Enabling and Commercializing</strong>
    1. Production feature development (DDR5/PCIe/Out-of-Band Management/RAS/Power & Thermal).
    2. Chip bringup in 72 hours.
    3. Enabling full machine in 1 month.
    4. Mass production in 12 months (EVT/PVT/DVT,Bugfix, chip workarounds).

#### Reference software stack:
<div>
    <img class="three" src="{{ site.baseurl }}/assets/img/YiTian710_Stack.png" alt="" title="YiTian710 Stack"/>
</div>
