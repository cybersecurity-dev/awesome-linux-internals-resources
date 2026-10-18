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
