# NimScan
Multi-threaded asynchronous port scanner written in Nim

## Benchmarks
![](gif/Scanner.gif)

## Tests
Nim Port Scanner Tested on:
- Windows 10 x64
- Kali Linux x64

## Usage
```Bash
./Scanner -p:<portX>-<portY> <host> [--timeout=<time>] [--showAll]
./Scanner -p:<port> <host> [--timeout=<time>] [--showAll]
./Scanner -p:<port1>,<port2>,<portN> <host> [--timeout=<time>] [--showAll]
```
## Examples
Scan range between 1 to 65535 ports

```Bash
./Scanner -p:1-65535 10.0.0.69
```

Scan specific ports
```Bash
./Scanner -p:80,443,445 10.0.0.69
```

Show also closed ports
```Bash
./Scanner -p:1-65535 10.0.0.69 --showAll
```
