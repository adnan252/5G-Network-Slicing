# 5g Network Slicing

Simulate and Analyze 5G Network Slicing using open-source software for different use-cases.

## Objectives

- To Understand the concept of 5G and Network Slicing.
- To Explore various simulation tools available for Network Slicing.
- To simulate 3 use-cases of 5G Network slicing.
- To analyze the results obtained from the simulation.

## Methodology

5G network slicing is the use of network virtualization to divide single network connections into multiple distinct virtual connections that provide different amounts of resources to a different type of traffic. RAN is the part of an end-to-end network that exists between the UE and the base station. The entire base station spectrum is divided to provide services to different applications using frequency division multiplexing. A base station has slices in it tailored for different needs such as,

- Guaranteed / Min bandwidth
- Max bandwidth
- Allocated throughput
- QoS class

![Image text](/Images/Picture1.png)

 Each slice in the base station/gNB has a different QoS Class which is based on the above-mentioned parameters. There are 3 types of slices with their corresponding QoS class defined as given below,

- Massive Machine Type Communications (mMTC)  - 2
- Ultra-Reliable Low Latency Communication (uRLLC)  -  1
- Enhanced Mobile Broadband (eMBB) -  3.
uRLLC is given top priority since it caters to time-critical applications with low latency requirements.
We made the necessary changes to the characteristics of a slice in a base station using the Slicesim simulation tool. 20 base stations with varied client sizes were used in the simulation. To simulate real-time conditions, multiple base station capacities and coverage areas were configured, and the related results were drawn.

## Results

![Image text](/Images/Picture2.png) ![Image text](/Images/Picture3.png)
![Image text](/Images/Picture4.png)

## Conclusion

In this project, we have simulated RAN slicing where the base station’s radio spectrum is divided to provide service to different use-cases. There are 3 main use cases currently mentioned in the standard to cater to a different set of users. RAN slicing is the main establishment between the use and the base station. It is the main part of the End-to-End slice as it creates the initial connection between the user and the base station and allocates the required bandwidth for each user based on the slice requested by the connected user. As a result, we investigated various simulation tools. We chose Slicesim from a variety of tools to simulate the 3 slicing use-cases and examine the various performance metrics.
