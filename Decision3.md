<a name="br1"></a> 

**Decision 3 - Backend Language**

**Decision: Node.js**

The choice of Node.js as the backend language was made aꢀer consideraꢁon of alternaꢁve opꢁons,

including Python and Ruby on Rails.

**Raꢀonale**

Node.js allows JavaScript to be running on both server-side and client-side, enabling full-stack JavaScript

development. It can handle asynchronous operaꢁons which allow us to process mulꢁple connecꢁons at

the same ꢁme. Its lightweight and fast execuꢁon environment results in low-latency responses and high

throughput. However, real-ꢁme capabiliꢁes require thorough design and scaling to handle heavy traﬃc

and loads. Development teams must be extremely proﬁcient in both front-end and back-end development,

which could aﬀect team composiꢁon.

While Python is renowned for its simplicity and readability, making it easy to maintain and develop, it does

not support full-stack JavaScript development. Ruby on Rails is known for its convenꢁon over conﬁguraꢁon

which allows rapid development ꢁme due to its clear project structure. This makes it an opꢁon for speciﬁc

projects if ꢁme is limited. However, it might not perform as good as Node.js when it comes to handling

real-ꢁme updates and concurrent connecꢁons.

**Consequences**

Node.js was chosen because of its strong real-ꢁme performance. It oﬀers an event-driven, lightweight,

and fast execuꢁon environment which is essenꢁal for managing mulꢁple connecꢁons eﬃciently and

delivering real-ꢁme updates such as order status, push noꢁﬁcaꢁon, data synchronizaꢁon, analyꢁc tools,

etc. Integraꢁon of various services such as linking APIs to our app, ﬁts the funcꢁonaliꢁes like the payment

system. By choosing Node.js, we aim to ensure that the app can deliver real-ꢁme services and handle the

expected loads eﬃciently. While both Python and Ruby on Rails have their advantages, Node.js is best

suited to our project’s needs.

Page | 7


