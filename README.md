# NTIA RAN Tester UE

This is a modification of srsRAN's UE software for use in security testing. It has enhanced metrics logging capabilites, and several attacks that can be launched against the RAN.

---

See the our comprehensive [documentation ](https://docs.rantesterue.org) for more info on our attacks and metrics.

## Quickstart Guide

1. Install Build Dependencies:

```bash
sudo apt-get update && sudo apt-get install -y cmake gcc g++ make libzmq3-dev libboost-all-dev \
    libuhd-dev uhd-host pkg-config libfftw3-dev libmbedtls-dev libsctp-dev libyaml-cpp-dev libgtest-dev
```

2. Clone the core repository:

```bash
git clone https://github.com/oran-testing/rtue.git
```
3. Build from Source:

```bash
cd rtue
mkdir build && cd build
cmake ../
make -j $(nproc)
sudo make install
```
