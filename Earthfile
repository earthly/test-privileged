locally:
    LOCALLY
    RUN hostname > /tmp/hostname.3d4b1831-c07e-4b2d-805e-2b8ce578bb50
    SAVE ARTIFACT /tmp/hostname.3d4b1831-c07e-4b2d-805e-2b8ce578bb50 hostname

regular:
    FROM alpine:latest
    RUN echo this should work > output
    SAVE ARTIFACT output

privileged:
    FROM alpine:latest
    RUN --privileged cat /proc/self/status | grep CapEff > output
    SAVE ARTIFACT output proc-status
