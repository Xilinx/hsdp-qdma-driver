# HSDP QDMA Driver
## Apply patch

1. `clone github.com/Xilinx/dma_ip_drivers`
2. `git apply hsdp_qdma_driver.patch`

## Install and setup driver

1. `cd dma_ip_drivers/QDMA/linux-kernel/driver/src/extra/scripts`
2. `./install.sh`
3. reboot
4. `dma_ip_drivers/QDMA/linux-kernel/driver/src/extra/scripts/setup.sh <bus number>`

## Run

1. `ls /dev/qdma*`
2. `hw_server -e "set dpc-pcie <qdma path above>"`

Copyright (C) 2023, Advanced Micro Devices, Inc.
