---
layout: home
title: Training Infrastructure as a Service
---

# Training Infrastructure as a Service

<img src="/assets/media/tiaas-logo.png" alt="tiaas logo depicting people in queues" width="300em" style="margin: 1em">

[UseGalaxy.eu](https://usegalaxy.eu) is proud to provide Training Infrastructure as a Service (TIaaS) for the Galaxy training community.
You provide the training, we provide the infrastructure <i>at no cost</i>.

## Why TIaaS?

- Private queue where only your training's jobs will run
- Free
- No Galaxy Maintenance
- No Galaxy Administration
- Official [Galaxy Training Materials](https://training.galaxyproject.org) are guaranteed to work and [regularly tested](https://github.com/usegalaxy-eu/workflow-testing/)
- See how your students are progressing with [our dashboard](/posts/2019/06/17/tiaas-queue/):

  ![tiaas queue visualizer](/assets/media/tiaas-queue.png)

## How TIaaS Works

We have several "pools" of VMs attached to UseGalaxy.eu that run user jobs. For
trainings we attach a new pool of VMs that is specially labelled for that
training. When normal users run tools on our server, these jobs are instructed
to avoid the training pools by default.

When users join a training, using a special URL we provide you, they then are
placed in a special training group. Their jobs will then preferentially run the
jobs on a training machine, and, in the event there is no more capacity, they
will run on the main queue. If a spot on a training VM opens up first, they
will run there rather than continuing to wait in the main queue.

## Eligibility

We have significant capacity and have dedicated some of this to providing
training using our service. Anyone providing training on using Galaxy is
eligible to request the use of this service.

## Service Level Agreement

We *cannot* promise any degree of uptime. We will do our best to have this service online and functioning during the entire time period but there are cases where the service may experience interruptions that are outside of our control. We will keep you informed of any outages that may affect your training.

## Application Process

1. Fill out the request form and we will get in touch with you

   {% include button.html url="https://docs.google.com/forms/d/e/1FAIpQLSdoPRDhpYwNFuZSlGRNQj3dDWwfsdemP5yntAdcqhN3YHbqLA/viewform" text="Request Training Infrastructure" %}

2. Together with you, we will determine how many VMs are needed for your training to run smoothly
3. We will setup the private queue and give you a URL your users will access to join the training.
