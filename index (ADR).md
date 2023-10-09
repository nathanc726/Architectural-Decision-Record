<a name="br1"></a> 

**Assignment: Architectural Decisions**

**Student Name:**

**Ho Pong Chan (Nathan)**

**Man Ho Cheung (Felix)**

**Chosen Scenario:**

**1 - Retail Company**

Page | 1



<a name="br2"></a> 

**Title**

Develop a new mobile app for a retail company.

**Status**

Approved.

**Context**

Our team has been invited to develop a new mobile applicaꢀon (app) for a retail company. The goal is to

enhance proﬁtability and expand the company’s global presence by improving user experiences through

the app. The app is designed to oﬀer the following features to customers:

·

·

·

·

browse products and view order history without an internet connecꢀon.

purchase products.

track order delivery status.

access and parꢀcipate in the loyalty program to earn and redeem points.

In addiꢀon to the funcꢀonaliꢀes for customers menꢀoned above, the retail company requires the

following funcꢀonaliꢀes that allow it to collect user data for business analysis and processing payments.

The data collected will be used and analyzed to design business strategies for business expansion on an

internaꢀonal scale. Data in the app must be synchronized with the server once internet connecꢀon is

available. The following are the funcꢀonaliꢀes that the retail company requires.

·

noꢀfy users about order updates, new product arrivals, exclusive oﬀers, and order delivery status

via push noꢀﬁcaꢀon.

·

·

·

integrate secured payment gateways.

track user behavior for business analysis and performance enhancement purposes.

implement image opꢀmizaꢀon techniques for product image display by choosing a suitable image

storage soluꢀon.

·

equip database to support mulꢀple languages and cultural preferences.

Page | 2



<a name="br3"></a> 

According to the above requirements given by the retail company, we will develop a mobile app with 6 key

components as follows.

**i.**

**Support oﬄine mode**

The retail company wants customers to be able to browse its products and view their order history

when the internet is not available. Having the app supported with oﬄine mode is a way to achieve

this feature. To ensure the downloaded database is updated, the app will be set to synchronize its

database with the server once an internet connecꢀon is available.

**ii.**

**iii.**

**iv.**

**Push noꢀﬁcaꢀon**

The retail company wants customers to be updated about its new product arrival, exclusion oﬀers,

order status, and order delivery status. Push noꢀﬁcaꢀons will be migrated to this app thus its

customers will be noꢀﬁed accordingly.

**Payment gateways**

Diﬀerent payment gateways will be integrated into this app to allow customers to pay for their

orders to facilitate secure and convenient payments. Credit card and third-party payment plaꢁorm,

named PayPal, will be used due to its security, ease of use, and compaꢀbility with this app.

**User behavior tracking**

The retail company wants to collect user behaviors in terms of product views, purchases, loyalty

program interacꢀon, etc. to improve app performance, enhance user experience, analyze user

data, and design business strategies. To achieve this, the tracking funcꢀon and analyꢀcs tool will

be migrated to this app.

**v.**

**Product image display**

Photos of all products need to be displayed to users. Since a higher level of user experience in

terms of aestheꢀcs is required, the size and resoluꢀon of photos need to be uniﬁed for easy

browsing and app opꢀmal performance.

Page | 3



<a name="br4"></a> 

**vi.**

**Mulꢀ-language**

Because of the goal of global business expansion, to avoid surﬁng diﬃculꢀes associated with

language barriers and cultural preferences for a high level of user experience, choices of language

will be available in the app.

To build this app, we made 6 architectural decisions that deﬁne the technology stack and approach for this

app development. These architectural decisions are developed based on the factors of performance,

maintainability, and scalability.

Page | 4



<a name="br5"></a> 

**Decision 1 - Mobile App Type**

**Choice: Naꢀve Mobile App**

Based on the needs of opꢀmal performance, device-speciﬁc features, and oﬄine funcꢀonality, the naꢀve

mobile app has been chosen.

**Raꢀonale**

A naꢀve mobile app was chosen due to its ability to deliver opꢀmal performance, leverage device-speciﬁc

features, and support oﬄine funcꢀonality. Naꢀve apps are plaꢁorm-speciﬁc, designed explicitly for iOS

and Android, enabling users to beneﬁt from plaꢁorm-speciﬁc capabiliꢀes, and ensuring smooth oﬄine

operaꢀon by eﬃciently managing device resources and data storage.

**Consequences**

**Pros**

Because of its opꢀmal performance and device-speciﬁc features such as oﬄine data and resource access,

users can access the locally stored content of the app in oﬄine mode.

**Cons**

Since iOS and Android are two diﬀerent Operaꢀng Systems, extra eﬀort and ꢀme are required for app

development when compared to cross-plaꢁorm soluꢀons. Maintenance costs may rise when, for instance,

ﬁxing bugs and updaꢀng the app system on two diﬀerent plaꢁorms.

Page | 5



<a name="br6"></a> 

**Decision 2 - UI Framework**

**Choice: React Naꢀve.**

React Naꢀve allows developers to write code in JavaScript for the interface which is working across both

iOS and Android plaꢁorms. Mulꢀ-language support can be built in within the user interface.

**Raꢀonale**

React Naꢀve can signiﬁcantly reduce development ꢀme and eﬀort due to the ability of code reuse. The

result of code updates can be seen in a real-ꢀme environment. The built-in component library brings ease

and eﬃciency for developers to build and maintain the user interface with choices of diﬀerent languages

which can be rendered on both iOS and Android plaꢁorms. React Naꢀve also provides internaꢀonalized

and localized libraries that enable the app to handle mulꢀple languages, including emojis.

**Consequences**

**Pros**

Both code and component library can be used in both iOS and Android Operaꢀng Systems which reduces

development ꢀme and eﬀort. Mulꢀ-language support enables the company to aꢂract users from various

regions with diﬀerent language and cultural backgrounds.

**Cons**

Although React Naꢀve oﬀers a wide range of naꢀve modules, it may not cover speciﬁc plaꢁorm-speciﬁc

features or APIs.

Page | 6



<a name="br7"></a> 

**Decision 3 - Backend Language**

**Decision: Node.js.**

The choice of Node.js as the backend language can handle real-ꢀme updates and integraꢀon of various

services due to its lightweight and eﬃcient performance.

**Raꢀonale**

Node.js allows an event-driven, lightweight, and fast execuꢀon environment that can eﬃciently handle

concurrent connecꢀons and real-ꢀme updates such as order status, push noꢀﬁcaꢀon, data

synchronizaꢀon, analyꢀc tools, etc. Integraꢀon of various services such as linking APIs to our app ﬁts the

funcꢀonaliꢀes provided in this app such as the payment system.

**Consequences**

**Pros**

Node.js allows JavaScript to be running on both server-side and client-side, enabling full-stack JavaScript

development. It can handle asynchronous operaꢀons thus several connecꢀons can be processed

simultaneously. Its lightweight and fast execuꢀon environment results in low-latency responses and high

throughput.

**Cons**

Real-ꢀme capabiliꢀes require thorough design and scaling to handle heavy traﬃc and loads. Development

teams must be extremely proﬁcient in front-end and back-end development knowledge, which could

aﬀect team composiꢀon.

Page | 7



<a name="br8"></a> 

**Decision 4 - Permissions**

**Decision: Granular permissions system**

A granular permissions system will be used in this app ensuring users have control of what data and device

features they can access. It also restricts the system from accessing sensiꢀve data of users.

**Raꢀonale**

Granular permissions allow users to conﬁgure the privacy and security level such as enabling the funcꢀon

of a push noꢀﬁcaꢀon, user of microphone, and locaꢀon, etc. when required for corresponding tasks. A top

priority of privacy and security and permission handling can be guaranteed and pracꢀced, respecꢀvely.

This system upholds user control.

**Consequences**

**Pros**

Protecꢀng user privacy enhances user trust and conﬁdence by implemenꢀng a granular permissions

system.

**Cons**

This system adds complexity to the development process. The development of a granular permissions

system requires careful system building otherwise incorrect conﬁguraꢀon may lead to privacy and security

risks and even leakage. If the restricꢀons are overly strict, it limits the app’s funcꢀonality which may

discourage users from using the app.

Page | 8



<a name="br9"></a> 

**Decision 5 - Data Storage**

**Decision: SQLite for local oﬄine storage and API for server-side data.**

Using SQLite for local oﬄine storage and API for service-side data balances oﬄine funcꢀonality with real-

ꢀme data updates.

**Raꢀonale**

A lightweight and eﬃcient database engine can be developed by SQLite for product data and order storage

locally. Data consistency can be ensured by using APIs for server-side data storage. Hybrid data storage

soluꢀons will be implemented to support both oﬄine and online mode operaꢀons. Synchronizing data

with the server will be completed instantly when the internet is available for the app to connect to.

**Consequences**

**Pros**

SQLite is a self-contained technology that does not rely on a separate service process that supports oﬄine

mode operaꢀon. It does not require complex setup or conﬁguraꢀon while being capable of working across

diﬀerent plaꢁorms. Using APIs allows the naꢀve app to access external services, data sources, and

funcꢀonaliꢀes without a complex setup. It also enables real-ꢀme data updates.

**Cons**

Data synchronizaꢀon between local SQLite database and remote APIs increases system complexity which

requires thorough design to avoid incorrect conﬁguraꢀon. Using APIs limited user controls (both the

company and customers) as those are owned and operated by other third parꢀes. Unexpected service

disconꢀnuaꢀon and/or limit adjustments and updates can signiﬁcantly impact the app’s behavior and

performance which lowers user experience and saꢀsfacꢀon. Storage capacity is solely dependent on users’

devices.

Page | 9



<a name="br10"></a> 

**Decision 6 - Addiꢀonal Frameworks or Technology Stacks**

**Decision: Firebase for push noꢀﬁcaꢀon, payment gateway, analyꢀcs integraꢀon.**

**Image Opꢀmizaꢀon by using the format of JPEG.**

Firebase provides a robust set of tools and services such as push noꢀﬁcaꢀons, payment gateway

integraꢀon, and analyꢀcs. The image format of JPEG is chosen for image opꢀmizaꢀon.

**Raꢀonale**

Firebase is a comprehensive tool to easily migrate diﬀerent funcꢀons (including analyꢀcs, message real-

ꢀme delivery, and payment) into the app that streamlines common mobile app features resulꢀng in a

reducꢀon of development eﬀort and ꢀme. Analyꢀc tools monitor user behavior and app performance and

help make data-driven decisions by having insights from user data. The format of JPEG maintains images

in high resoluꢀon with a lower ﬁle size. With the use of JPEG image format, images can be opꢀmized for

browsing, loading, and storage.

**Consequences**

**Pros**

Push noꢀﬁcaꢀon, analyꢀcs, and payment gateway provided by Firebase can work across diﬀerent

plaꢁorms resulꢀng in implementaꢀon simplicity. Firebase’s security features help protect sensiꢀve

payment informaꢀon by using data encrypꢀon and compliance with Payment Card Industry Data Security

Standard requirements [1]. Analysis generated by analyꢀc tools provides detailed insights into user

behavior and app usage etc. help ﬁne-tune and further develop the app. Image opꢀmizaꢀon leads to

higher loading and storage eﬃciency that reduces the load on both user devices and servers while

maintaining relaꢀvely high image resoluꢀon. A beꢂer browsing experience can be delivered to users,

especially where bandwidth and storage constraints occur.

Page | 10



<a name="br11"></a> 

**Cons**

The cost of using Firebase can be very high if the usage volume such as frequent payment processing is

large. Since event tracking is enabled in the app (when the user enables this funcꢀon), improper handling

of user data can result in legal and reputaꢀon issues. Clear, logical, and strict data governance is solely

dependent on how the company designs it. If improper government is set, user’s privacy and data cannot

be safeguarded. JPEG does not support lossless compression. If the image is heavily compressed, the loss

of quality is noꢀceable.

Page | 11



<a name="br12"></a> 

**Conclusion**

In this Architectural Decision Report, the essenꢀal choices guiding the development of a new mobile app

for a retail company are laid out. These decisions include the app’s funcꢀonality and technology stack

which align with the project’s goals.

We have chosen a naꢀve mobile app that prioriꢀzes opꢀmal performance and oﬄine funcꢀonality. React

Naꢀve will be used for the UI framework which runs across mulꢀple plaꢁorms. Node.js is selected for back-

end technology because of the advantages of its real-ꢀme capabiliꢀes and service integraꢀon. A granular

permissions system can protect sensiꢀve data security while leaving control to the user. A hybrid approach

of using both SQLite for local storage and APIs for server-side data ensures seamless data synchronizaꢀon.

Firebase handles and processes push noꢀﬁcaꢀons, payment gateway integraꢀon, and analyꢀcs. Image

Opꢀmizaꢀon associated with using the JPEG image format helps streamline photo processing and loading

which enhances user experience. With all the decisions made in this report, the app is correctly posiꢀoned

for the retail company to meet its goal of global business expansion and proﬁtability. The main objecꢀve

achieved by this app is to enhance the user experience. With this posiꢀve impact, revenue can be pushed

up to a higher level which increases ﬁnancial assets to expand its business internaꢀonally.

Page | 12



<a name="br13"></a> 

**References**

1

N. Barney. “PCI DSS (Payment Card Industry Data Security Standard.” TechTarget. Accessed:

October 7, 2023. [Online.] Available: hꢂps://www.techtarget.com/searchsecurity/deﬁniꢀon/PCI-

DSS-Payment-Card-Industry-Data-Security-

Standard#:~:text=The%20primary%20goal%20of%20PCI,breaches%2C%20fraud%20and%20iden

ꢀty%20theꢃ.

Page | 13

