Mục đích
=====

hiểu cách hoạt động của giao thức AMQP. 

sử dụng được rabbitmq với kombu(hoặc pika)


AMQP
=====
* Advanced Message Queuing Protocol
* Là một giao thức mạng, tầng ứng dụng cho phép các ứng dụng clients giao tiếp
với middleware broker

AMQP 0-9-1 model
-----
* Là mô hình AMQP có kiến trúc như sau:
    Publisher đưa ra các messages đến Exchanges, exchanges phân tán các bản copy 
    của message nhận được đến các queue sử dụng các nguyên tắc phân bố gọi là binding 
    sau đó message broker sẽ chuyển các messages đó đến consumers hoặc consumer tự lấy

* Queues, exchanges, bindings được gọi là AMQP entities 

Messaging Broker
-----
* Nhận message từ producer và chuyển đến consumer.






