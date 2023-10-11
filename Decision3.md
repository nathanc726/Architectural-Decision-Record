<a name="br1"></a> 

**Decision 3 - Backend Language**

**Decision: Node.js**

The choice of Node.js as the backend language was made after consideration of alternative options, including Python and Ruby on Rails.

**Rationale**

Node.js allows JavaScript to be running on both server-side and client-side, enabling full-stack JavaScript development. It can handle asynchronous operations which allow us to process multiple connections at the same time. Its lightweight and fast execution environment results in low-latency responses and high throughput. However, real-time capabilities require thorough design and scaling to handle heavy traffic and loads. Development teams must be extremely proficient in both front-end and back-end development, which could affect team composition.
While Python is renowned for its simplicity and readability, making it easy to maintain and develop, it does not support full-stack JavaScript development. Ruby on Rails is known for its convention over configuration which allows rapid development time due to its clear project structure. This makes it an option for specific projects if time is limited. However, it might not perform as good as Node.js when it comes to handling real-time updates and concurrent connections.


**Consequences**

Node.js was chosen because of its strong real-time performance. It offers an event-driven, lightweight, and fast execution environment which is essential for managing multiple connections efficiently and delivering real-time updates such as order status, push notification, data synchronization, analytic tools, etc. Integration of various services such as linking APIs to our app, fits the functionalities like the payment system. By choosing Node.js, we aim to ensure that the app can deliver real-time services and handle the expected loads efficiently. While both Python and Ruby on Rails have their advantages, Node.js is best suited to our project’s needs.

Page | 7


