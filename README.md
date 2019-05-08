# BCX19 Mobility Challenge

* [Bosch Connected Experience website](https://bosch-connected-world.com/hackathon/mobility/)

* When: Monday, May 13 to Wednesday, May 15 2019
* Where: [Kühlhaus Berlin](https://goo.gl/maps/qGVMvogz7xYL7qDH6) **5th floor**

![HackMC Area](images/hack_mc_area_plan.png)


## Available hardware

### E-Bikes with COBI.Bike

![COBI.Bike logo](https://pbs.twimg.com/profile_images/535863826529271808/_Zy4iyJ3_200x200.png)
![COBI.Bike system](images/cobi_system.jpg)
![COBI.Bike picture](images/cobi_image.jpg)

* Available: 3x E-Bikes with COBI.Bike unit and smartphones in HackMC area
* Contact person: _coming soon_

* COBI.js interfaces: https://cobi-bike.github.io/COBI.js/
* Chrome Simulator: https://chrome.google.com/webstore/detail/cobibike-devkit-simulator/hpdhkapigojggienmiejhblkhenjdbno 

#### Which data is available?

* Data from eBike Drive Unit
  * Battery range, odometer, assistance modes
* Sensors embedded in mobile device
  * GPS, Gyroscope, accelerometer
* External sensors
  * Heart rate, cadence, speed
  
#### How to access data?

COBI.js - a JavaScript library that abstracts the Bluetooth connections, authentication or CAN BUS and allows the developer to focus on the data

#### How to interact with the device or the system?

The COBI.Bike app and Hub: https://cobi.bike/product 

#### What events are available?

* Developers can subscribe to the streams of data they wish to access



### Eclipse Kuksa RC Rovers

![Eclipse Kuksa](images/eclipse_KUKSA.png)
![Rover](images/eclipse_kuksa_rover.png)

* Available: 3x Rovers in HackMC area
* Contact person: _coming soon_

#### Which data is available?

E.g. (live) Sensor Data 
* Camera
* Gyroscope
* Ultrasonic sensors
* Infrared sensors
* Temperature
* Humidity

#### How to access data?

* Retrieve data from database (where it was stored through Eclipse Hono)
* Sending data to vehicle via HONO to vehicle API

#### How to interact with the device or the system?

* Send data to hosted Eclipse Hono instance
* Eclipse hawkBit and connected App-Store
* Eclipse Che instance to implement applications

#### What events are available?

* App development and deployment 
* Push notifications
* Command & control of Rover

#### Useful links

* https://www.eclipse.org/kuksa/
* https://www.eclipse.org/kuksa/resources/
* https://app4mc-rover.github.io/rover-docs/

Programmable dongle to access vehicle diagnosis port.
Currently we work on integrating authorization flows into Eclipse Kuksa



### EV Challenge Jaguar I-PACE

* Available: 1x Jaguar I-PACE in front of building
* Contact person: _coming soon_

CAN Bus data available over HTTP

_more information coming soon_

### Anki Overdrive

* Available: 1x Track in the HackMC area with 4 cars
* Contact person: Pedro Silva

_more information coming soon_

### Audi e-Tron brake data

* Not physically available, only data access on demand

Ask the Bosch IoT Insights Hack Coaches




## Available software services

### Bosch IoT Suite

![Bosch IoT Suite](images/bosch_iot_suite.jpg)

Devices are typically connected to the Bosch IoT Hub, which pushed data to Bosch IoT Things. Changes of Things are recorded by Bosch IoT Insights and preserved for further analysis.

* **Bosch IoT Insights**

  The easy way to manage your IoT device data<br>
  https://bosch-iot-insights.com

* **Bosch IoT Things**
  
  Managed inventory of digital twins for IoT device assets

* **Bosch IoT Hub**
  
  Easy and secure device connectivity for the IoT

[Book your free plan](https://accounts.bosch-iot-suite.com/subscriptions/)

Find our Hack Coaches on the Marketplace on the 2nd floor.


### Here.com Telematics API

TBD: Logo, Description

* Contact person: _coming soon_

https://developer.here.com/documentation/fleet-telematics/dev_guide/topics/use-cases.html


### Axel Springer: Clever Tanken API

#### Which data is available?

* Gas stations (address, opening hours, div. features)
* Gas prices
* Car wash facilities

#### How to access data?

* Clever Tanken API
* Hack coach provides credentials 


#### Ideas

* OnMyWay: An app that shows the user where on his/her way the next e.g. McDonalds, Sanifair, Rewe, baby changing table, kids playground etc. is
* Gas price trend prediction


### Axel Springer: upday API

#### Which data is available?

* Top News Teaser (between 9 and 11)
  * URL to original source, image URL
  * title, preview text
  * publish time
  * category
  
* this is live news data
* it is available for 10 locales, curated by several editorial teams
* it is updated irregularily whenever something interesting or relevant happens
* the content of the specific locales differs
* valid locales are: de-DE, de-AT, de-CH, nl-BE, nl-NL, fr-FR, pl-PL, en-GB, es-ES, it-IT


#### How to access data?

Requests to REST API:

    curl -u 'api:<pw>' http://boschhackathon.topnews.upday.com/api/v1/top-news/{locale}

Password provided by Hack Coach


### TIBCO
<p align="center">
  <img width="50%" height="50%" src="https://github.com/TIBCOSoftware/flogo/raw/master/images/projectflogo.png">
</p> 
Project Flogo is a go-based open source ecosystem for building event-driven apps and has the notion of triggers and actions to process any incoming event.
<p align="center">
  <img  src="https://github.com/TIBCOSoftware/flogo/raw/master/images/eventhandlers.png">
</p>

#### When to use Flogo?
If you’re dev & sick of building all the messy stuff that comes along with coding production apps, such as connectivity to event-driven messaging platforms, datastores, SaaS apps, etc & want to deploy to a wide range of targets, such as

* serverless compute
* IoT edge devices
* containers

then Project Flogo is for you!

#### How to access data? 
You can use one of our triggers to receive data. Examples triggers are:
* Kafka, MQTT, CoAP, REST, GraphQL, AWS Lambda, Timer, AMQP ...and many others

You can use one of our actions to process or send data back. Examples activities are: 
* Log, MQTT, Kafka, AMQP, Trello, Write to File, Pushbullet, Tensorflow, IFTTT, AWS S3, RasPi GPIO

...and you can contribute in the development of new triggers and activities as well.

#### How to get Project Flogo?
Project Flogo can be downloaded from github and more details can be found here 
https://github.com/tibcosoftware/flogo

A Web UI to develop with a zero-code approach is available via Docker (highly recommended for the Hackathon):
https://hub.docker.com/r/flogo/flogo-docker

You can run Flogo on your laptop, on a edge device like a RasPi, on a container like OpenShift or even on AWS Lambda 

The Flogo Web UI comes along with all required components to begin developing, testing and building deployable artifacts from your web browser.

![](https://github.com/TIBCOSoftware/flogo/blob/master/images/flogo-web2.gif)

Find our Hack Coaches on the Marketplace on the 2nd floor. We show you how to connect to the Bosch IoT Hub, receive device messages and build something cool!


### Red Hat

TBD


### Mathworks

Get a Matlab license for the hackathon and get support from the Hack Coaches.

TBD

