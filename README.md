# APB-implementation-for-FPGA
This repository consists of all the related files for my B.Tech major project.<br>
Included files-<ul><li>Presentation</li><li>Report</li><li>Source code</li><li>UCF file for FPGA</li></ul><br><hr>
<h2>How to use</h2>
I have provided the source code (not very optimized) but still works fine. My targeted device was Nexys 3 FPGA board which has 8 switches so instead of using 8 bits for data to be written, i've restricted it to 2 bits. Same with read and write address but didn't have switches available, so I assigned pre-defined values for them.<br>
To see the switches and LEDs mapping, you can refer to the presentation provided, it has a slide dedicated on my mappings or UCF file can also be referred.<br>
Paste the source code in Xilinx ISE, Vivado or relevant FPGA tool and map the ports (UCF file in ISE or XDC file in VIVADO) to relevant hardware available in your targeted board, generate the bitstream file and dump into board. Be mindful, if the FPGA board only has RAM, like Nexys 3, then it'll lose the bitstream file when disconnected.<br>

<br>I have added some additional signals which aren't the part of actual protocol because some were necessary for the scope of the project others beacuse I didn't knew how to solve the problems that'd arise without it. But I'm working to make a more efficient version of this project.
