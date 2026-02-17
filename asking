### How to ask

## Subject: Architecture Check: Docker vs. rkt On-Disk Storage

Hi everyone,

I’m verifying my understanding of container storage internals and would appreciate a quick sanity check on my comparison:

Docker: Uses Content-Addressable storage and Union Filesystems (Overlay2). It layers read-only images with a thin writable layer on top for space efficiency.

rkt: Uses the App Container (appc) spec. It renders a more self-contained rootfs within a Pod structure, prioritizing isolation over shared-layer complexity.

My Take: Docker’s design seems optimized for deployment speed/disk density, while rkt’s design prioritizes security boundaries and pod-level composability.

Does this accurately represent the core architectural trade-offs between the two, or am I missing a key technical nuance in how they commit data to disk?

Best,

[Your Name]
