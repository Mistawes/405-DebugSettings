# 4.05 kernel dumper POC with debug settings/TID patch/Jailbreak/Uart enabler etc

Compile with your PC's IP listening on port 9023

On PC you can do to listen:
	socat - tcp-listen:9023 > kernelDump.bin

and to send:
	socat -u FILE:payload.bin TCP:"PS4 IP":9020

you can then trim out the socket prints or you can adapt it with 2 sockets, one for dumping, another for logging.


