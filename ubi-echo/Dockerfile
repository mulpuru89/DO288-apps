FROM registry.access.redhat.com/ubi8/ubi:8.0
RUN mkdir test
COPY build.sh test/
RUN chgrp 0 /test && chmod g+rwx /test
USER 1001
CMD bash -c "while true; do echo test; sleep 5; done"
