F‑STATIC — High‑Performance Static File Server
F‑STATIC is a lightweight, zero‑allocation static file server designed for extreme throughput and low latency. Files are preloaded into RAM and served through a single epoll‑driven event loop, enabling exceptional performance even on modest hardware.

LICENSE:
JakeServer is released under the MIT License. This allows free use, modification, distribution, and commercial use of the software. See the LICENSE file for full details.

FEATURES:
• RAM‑preloaded files for instant response times
• Single‑threaded epoll loop for efficient concurrency
• Zero allocations per request
• 20k+ requests per second on older CPUs
• Low CPU usage under heavy load
• Simple command‑line UI for adding and listing files
• Ideal for static sites, assets, and CDN‑style delivery

QUICK START:

Download the latest release

Unzip the package

Run the server: ./jake_server

Add files to RAM: add /index.html ./webroot/index.html

Start serving: start

HOW TO RUN:
1.JakeServer is a Linux‑based static server and must be run through the Linux terminal.

2.Extract the ZIP

3.Open a terminal in the extracted folder

4.Make the server executable: chmod +x jakeserver

5.Run it: ./jakeserver

PERFORMANCE:
Benchmark example (FX‑series CPU):
• 24,168 requests/sec
• ~1.9 ms average latency
• 21.48 MB/sec transfer rate
• Zero socket errors under load

IMPORTANT NOTE:
Linux open‑file and open‑socket limits can restrict stability above ~20k concurrent users.
If you need high stability and high user counts per machine, you MUST increase these limits.

These results demonstrate F‑STATIC’s ability to handle large volumes of legitimate traffic with minimal resource usage.

USE CASES:
• Static websites
• CDN‑style asset delivery
• Embedded systems
• High‑throughput microservices
• Local development servers
• Performance research and experimentation

LICENSE:
This project is released under the MIT License. See the LICENSE file for details.
