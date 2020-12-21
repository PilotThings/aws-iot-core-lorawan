# AWS IoT Core for LoRaWAN sample applications 
AWS IoT Core for LoRaWAN enables you to setup a private LoRaWAN network by connecting your devices and gateways with no LoRaWAN Network Server setup required.

In this repository  you will find fully functional sample applications to quickly get started developing solutions using AWS IoT Core for LoRaWAN. Please also consider our [developer guide](https://docs.aws.amazon.com/iot/latest/developerguide/connect-iot-lorawan.html) to learn how to connect your wireless devices and gateways to AWS IoT Core for LoRaWAN.

# Sample applications

- [A "Hello world" application: decoding LoRaWAN binary payloads using AWS IoT Rules and AWS Lambda](transform_binary_payload)  
    LoRaWAN devices typically send uplink payloads as binary encoded messages. In this sample you will learn how to decode a binary message from your LoRaWAN device and republish the decoded payload to the MQTT topic of AWS IoT Core. To support you in implementation of more advanced use cases, this sample contains two additional optional sections: guidelines on how to use AWS IoT Rules to integrate the decoded payload with more then 17 AWS services, and guidelines on how to build and deploy a binary decoder for your LoRaWAN device.  

- [Analyzing LoRaWAN payloads with Amazon Timestream and visualizing them with Grafana timestream plugin](timestream)  
    In this sample you will use AWS IoT Core for LoRaWAN and AWS IoT Core to ingest time series data from your LoRaWAN devices into Amazon Timestream. Once your data are stored in Amazon Timestream, you can visualize your data in Grafana using a [Grafana timestream plugin](https://grafana.com/grafana/plugins/grafana-timestream-datasource/installation). This repository explains how to build a sample solution for storing and visualizing your times series data.

- [Monitoring and alarming of soil moisture by using AWS IoT Core for LoRaWAN and AWS IoT Events](soilmoisture_alarming)  
    Detecting events based on telemetry data from connected devices is a common use case in IoT across many industries. This sample explains how to integrate AWS IoT Events with LoRaWAN for IoT Core. You can learn how to translate telemetry values from a LoRaWAN device into events and notify users about these events using E-Mail and SMS.

# Getting help 
- [API Reference](http://docs.aws.amazon.com/console/iot/wireless/intro/apiref)
- [Developer guide](http://docs.aws.amazon.com/console/iot/wireless/intro/devguide)
- [FAQs](https://aws.amazon.com/iot-core/faqs/#AWS_IoT_Core_for_LoRaWAN)
- [Support forums](https://forums.aws.amazon.com/forum.jspa?forumID=210)
- [Partner catalog](https://devices.amazonaws.com/search?page=1&sv=iotclorawan)
