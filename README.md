## Hi there 👋
I'm Elias Paitz, aka LightJack05. Welcome to my GitHub Profile!

## Who am I?
I am a technology enthusiast from Germany. 
I specialize in eliminating Toil from setups and making sure they run reliably.
Additionally, I attempt to create platforms that make other people's (and my) life easier and more efficient.

On the side, I also recently started doing some embedded dev, an example of which you can check out [here](https://github.com/LightJack05/meme-pi).

## Reference Projects
If you're here to see some projects, take a look at the ones below.

### My private cloud under my desk (My HomeLab v2)
Over the past years, I have moved on from just making things work, and started to make things efficient.
I ended up simplifying a VM deployment and also configuration management to just 10 lines of YAML + additional playbooks aside from the base config:

```yaml
deployments:
  - name: "OS-Webserver-1"
    node: 4
    num_cpus: 2
    num_mb_ram: 4096
    ipv4_address: "10.130.0.5/16"
    ipv4_gateway: "10.130.0.1"
    ipv4_dns: "10.130.0.1"
    interfaces:
      - vnet: "vnlabg"
```

Want to see how it works? Check out my [HomeLab-v2 repo](https://github.com/LightJack05/HomeLab-v2/)

### Embedded development of Kernel Modules
As a bit of a work-in-progress, I am currently working on building a Kernel module that serves as a Driver for an SPI epaper display and exposes an ioctl and mmap based interface for commands and framebuffer to userspace.

Take look around under my [meme-pi repo](https://github.com/LightJack05/meme-pi).

### Tooling and automation

#### Go License Collector
I replaced the deprecated Go License tool with a little bit of AI-Coded script.
It's very handy for managing licenses in Go projects, so you don't have to deal with it. On pretty much every PR in a Go Project, I run this tool to validate that all required licenses are present and up-to-date.

See [this repo](https://github.com/LightJack05/go-license-collector) for details.

#### Gitea Auto Mirror
I have built a tool that listens to github repo create events and adds push-mirror entries to the newly created repo in order to allow it to be mirrored to a different server.
(Should also work with Forgejo, but no guaruantees)

Take look at the code [here](https://github.com/LightJack05/gitea-auto-mirror) and [read the docs](https://lightjack05.github.io/gitea-auto-mirror/) if you are interested.

## Currently learning
### Talos and Kubernetes Operators
I'm currently diving deep into Talos systems, aiming to use it to replace my current Proxmox Hypervisor for more automation potential.
In the process, I will build on top of KubeVirt to enable virtualization on Talos.

My Bachelors Thesis project is planned to be a Kubernets operator allowing me to manage my VM hosted on KubeVirt using Ansible via the Kuberentes API.
Details on that will follow, so stay tuned!

## How to reach me
Select your favourite platform:
- [LinkedIn](https://www.linkedin.com/in/elias-paitz-a1779a334/)
- [Mail](mailto:eliaspaitz05@gmail.com)
- Discord: @lightjack05

## Fun Facts
- I love coffee
- I hate Toil and manual work
- I'm terrible at remembering names
- I use Arch btw.
- I use NeoVim btw.
