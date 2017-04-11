# springcloud_sample
springcloud例子

依次启动eureka-server1->eureka-server2->api-gateway1->api-gateway2->compute-service->compute-service2->compute-service3->service-B1->service-B2

访问服务a的测试链接
http://localhost:5555/api-a/add?accessToken=aa&a=1&b=2

访问服务b的测试链接
http://localhost:5555/api-b/select?accessToken=aa

分别多访问几次, 查看打印结果.能看得出来, 在几次节点之间轮询.实现了负载均衡.