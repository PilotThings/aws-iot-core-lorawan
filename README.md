# AWS IoT Core for LoRaWAN sample applications 
AWS IoT Core for LoRaWAN enables customers to connect wireless devices that use low-power, long-range wide area network (LoRaWAN) technology and leverage the richness of AWS platform to build solutions based on the data ingested from these LoRaWAN devices.  Using AWS IoT Core for LoRaWAN, enterprises can setup a private LoRaWAN network by connecting their own LoRaWAN devices to the AWS Cloud - without developing or operating a LoRaWAN Network Server (LNS).
# How to get started
**1. Select the LoRaWAN wireless devices**  
    AWS IoT Core for LoRaWAN supports 1.0.x and 1.1 specifications standardized by LoRa Alliance. Supported LoRaWAN devices classes are A, B and C. 

**2. Select the LoRaWAN gateways**  
    AWS IoT Core for LoRaWAN supports [open-source](https://github.com/lorabasics/basicstation) gateway software [LoRa Basics Station](https://lora-developers.semtech.com/library/tech-papers-and-guides/how-to-use-lora-basics-station/). The [AWS Partner Device Catalog](https://devices.amazonaws.com/search?page=1&sv=iotclorawan) contains gateways and developer kits that are qualified for use with AWS IoT Core for LoRaWAN.  

**3. Add your wireless devices and LoRaWAN gateways to AWS IoT Core for LoRaWAN**  
    [Adding LoRaWAN gateways and devices](https://docs.aws.amazon.com/iot/latest/developerguide/connect-iot-lorawan.html#connect-iot-lorawan-getting-started-overview) describes how to add your wireless devices and LoRaWAN gateways to AWS IoT Core for LoRaWAN. 

**4. Start building your LoRaWAN solution** based on AWS IoT Core for LoRaWAN by using fully functional sample applications in this repository.  
# Sample applications

- [Decoding LoRaWAN device binary payloads and integrating them with other AWS services by using AWS IoT Rules](transform_binary_payload)  
    LoRaWAN devices typically send uplink payloads as binary encoded messages. In this sample you will decode binary messages from your LoRaWAN device by using AWS Lambda. After decoding, you will configure AWS IoT rules to integrate decoded LoRaWAN device payloads with more than 15 AWS Services (e.g. AWS IoT Sitewise, AWS IoT Events and Amazon Timestream).  

- [Analyzing LoRaWAN payloads with Amazon Timestream and visualizing them with Grafana timestream plugin](timestream)  
    In this sample you will use AWS IoT Core for LoRaWAN and AWS IoT Core to ingest time series data from your LoRaWAN devices into Amazon Timestream. Once your data are stored in Amazon Timestream, you can visualize your data in Grafana using a [Grafana timestream plugin](https://grafana.com/grafana/plugins/grafana-timestream-datasource/installation). This repository explains how to build a sample solution for storing and visualizing your times series data.

- [Monitoring and alarming of soil moisture by using AWS IoT Core for LoRaWAN and AWS IoT Events](soilmoisture_alarming)
    Detecting events based on telemetry data from connected devices is a common use case in IoT across many industries. This sample explains how to integrate AWS IoT Events with LoRaWAN for IoT Core. You can learn how to translate telemetry values from a LoRaWAN device into events and notify users about these events using E-Mail and SMS.
