# Electrical-appliance-monitoring-system

## Introduction

- The system of this project uses a non-invasive method to analyze the state of the user's electrical appliances in real time. The analysis interface includes the appliances currently in use, real-time total power, total duration of use for each appliance, and total power consumption.

- In terms of hardware, the current and voltage transformer is used to sample according to the fixed ratio and then the phase is adjusted by capacitance and sent to the analysis and identification module. The module adopts the domestic multi-functional and high-precision three-phase electric energy measurement chip HT7038, which calculates the parameters of active power and reactive power and then sends them to the single chip microcomputer for analysis. In order to better test the function, the team made two electrical appliances with similar characteristics for analysis and identification.

- In the software, the K-nearest neighbor algorithm (KNN) is selected on the identification of electrical appliances to identify the current electrical appliance combination, and then the cumulative use time, cumulative power consumption, real-time total power and electrical appliance type are calculated through the single-chip microcomputer timing and other functions to send to the serial screen and display, so as to achieve non-invasive electrical appliance monitoring function.

## Background

- Non-invasive electrical appliance monitoring is an intelligent technology for home, commercial or industrial environments, designed to monitor and analyze the energy consumption and working status of electrical appliances in real time, providing effective power management and optimization solutions. Traditional power monitoring methods usually require circuit intervention and installation of sensors, while non-invasive electrical appliance monitoring uses non-contact methods for data collection and analysis.

- With the increasing cost of energy and the increasing concern about energy consumption, the monitoring of electrical appliances has become an important technical requirement. Through non-invasive appliance monitoring, users can obtain detailed information about the actual energy consumption, operating status and usage patterns of appliances, thereby improving energy efficiency, reducing energy costs and reducing environmental impact.

## Engineering Goal

-  Reduce operating costs: real-time monitoring of electrical power consumption can help enterprises reduce energy consumption and operating costs, identify energy consumption peaks and valleys, and reasonably adjust equipment use time and mode, which can save energy and reduce energy costs.

- Improve safety and reliability: Electrical monitoring systems can help enterprises improve the safety and reliability of electrical equipment and reduce potential safety risks and accidents. This helps keep employees and assets safe and avoid downtime and losses due to electrical failures.

## Project Pipeline
![图片](https://github.com/HsAlex20/Electrical-appliance-monitoring-system/assets/111621662/2e6f63b5-5546-4781-a20a-84d0604df377)

## Summary of Procedure

- Learning mode. The current electrical parameters are read by spi and stored in an array.

- Analysis pattern. By comparing the parameters, the knn algorithm is used to get the usage of each electrical appliance.

- Switch modes by touching the serial screen to send back indicators.

- Use a timer to record the use time of each electrical appliance, and calculate the electricity consumption with various parameters.

## Significance

- Electrical appliances monitoring in industrial parks: By calculating the cumulative electrical energy of electrical appliances such as manufacturing tools, the cost of products can be better evaluated, and help to improve the production of products. When the electrical appliance is close to its design life, the user can consider maintenance or replacement to avoid failure; The power factor can be monitored, the energy efficiency of appliances can be assessed, and measures can be taken to reduce energy consumption and become greener.

- Online status monitoring of key instruments: identify the switch status of electrical appliances through algorithms, display the name of electrical appliances that are working, give early warning to electrical appliances that cannot be tested by personnel or need to be used for a long time, such as medical rescue instruments and temperature control instruments, and prevent property casualties, losses, and disasters caused by electrical failure and shutdown.

- Electrical fire prevention: The electrical monitoring system can monitor the factors that are prone to electrical fires, and the real-time display of power through Bluetooth can achieve uninterrupted data monitoring and statistical analysis of the factors that are prone to electrical fires, so that users can monitor the electricity consumption and prevent electrical hazards.

## Future Research

- Through the Internet of Things sensor terminal, the power data of electrical appliances can be transmitted to the virtual power plant cloud platform in real time, and the data can be efficiently transmitted from the field to the cloud and from the cloud to the system. At the same time, the data is analyzed and processed by AI to form a statistical analysis of the classification, sub-item, time-sharing and sub-region of the park's electricity consumption, and comprehensively and real-time display of the park's power use through visualization technology, intuitively find the power problems, help the park optimize the power use, reduce the park's comprehensive energy consumption, and achieve the visible, quantifiable, manageable and controllable power consumption goal of the enterprise. Moreover, the cloud platform controls intelligent electrical equipment, saves manpower and material resources, and reduces unnecessary energy consumption. It can be used in different scenarios such as apartments, hotels, factories, and medical treatment.

## Reference

[1]郭永贞,许其清,袁梦等. 数字电子技术[M].南京东南大学出版社:, 201806.372.

[2]郭立强. 电子技术基础简明教程[M].南京大学出版社:, 202008.303.

[3]江冰,林善明,江琴等. 模拟电子技术及其应用[M].南京大学出版社:, 201912.266.

[4]沈显庆,张秀,郑爽等. 开关电源原理与设计[M].南京东南大学出版社:, 201212.223.
