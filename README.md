```mermaid
flowchart TD
    A[User Applications] --> B["System Libraries<br/>glibc, libpthread"]
    B --> C[System Call Interface]

    subgraph Kernel Space
        C --> D[Process Management]
        C --> E[Memory Management]
        C --> F["Virtual File System (VFS)"]
        C --> G[Networking Stack]
        C --> H[IPC & Signals]
        C --> I[Security Framework]

        F --> J[Ext4 / XFS / Btrfs]
        G --> K[TCP/IP]
        G --> L[Netfilter / Firewall]

        D --> M[Scheduler]
        E --> N[Virtual Memory]
    end

    subgraph Device Layer
        O[Character Drivers]
        P[Block Drivers]
        Q[Network Drivers]
    end

    D --> O
    E --> P
    G --> Q

    O --> R[Hardware]
    P --> R
    Q --> R

    style A fill:#d4f1f9
    style B fill:#d4f1f9
    style C fill:#ffeaa7
    style R fill:#ff7675,color:#fff
```

# Awesome Linux Internals Resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://elixir.bootlin.com/linux/v6.17/source)
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)]()
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/r/linuxadmin/new/)

<p align="center">
    <a href="https://github.com/cybersecurity-dev/"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/github.svg" alt="GitHub"></a>
    &nbsp;
    <a href="https://www.youtube.com/@CyberThreatDefense"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/youtube.svg" alt="YouTube"></a>
    &nbsp;
    <a href="https://cyberthreatdefence.com/my_awesome_lists"><img height="20" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/blog.svg" alt="My Awesome Lists"></a>
    <img src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/bar.gif">
</p>

## 📖 Contents
- [My Other Awesome Lists](#my-other-awesome-lists)
- [Contributing](#contributing)
- [Contributors](#contributors)

##

### My Other Awesome Lists
You can access the my other awesome lists [here](https://cyberthreatdefence.com/my_awesome_lists)

### Contributing
[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors
[Thanks goes to these contributors](https://github.com/cybersecurity-dev/awesome-linux-internals/graphs/contributors)!

### License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

[🔼 Back to top](#awesome-linux-internals-resources-)
