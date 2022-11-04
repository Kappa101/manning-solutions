# manning-solutions

# project 1 solutions

## 
```http request
http://localhost:4070/api/flights/clusters/itineraries?from=BUE,MIA&to=MIA,BUE&departure=2023-05-29,2023-06-03&adults=1&children=1&infants=1&amount=10


{
    "id": "TWA_g=2022-11-04T18:45:53.880738_f=BUE,MIA_t=MIA,BUE_d=2023-05-29,2023-06-03_a=1_c=1_i=1",
    "pagination": {
        "offset": 0,
        "limit": 10,
        "total": 0
    },
    "itineraries": []
}

```


---
* logs 

```text

2022-11-04 18:45:28.915  WARN 31708 --- [           main] JpaBaseConfiguration$JpaWebConfiguration : spring.jpa.open-in-view is enabled by default. Therefore, database queries may be performed during view rendering. Explicitly configure spring.jpa.open-in-view to disable this warning
2022-11-04 18:45:28.981  INFO 31708 --- [           main] o.s.s.concurrent.ThreadPoolTaskExecutor  : Initializing ExecutorService 'applicationTaskExecutor'
2022-11-04 18:45:29.809  INFO 31708 --- [           main] o.s.b.a.e.web.EndpointLinksResolver      : Exposing 14 endpoint(s) beneath base path ''
2022-11-04 18:45:29.860  INFO 31708 --- [           main] o.e.j.s.h.ContextHandler.application     : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-11-04 18:45:29.861  INFO 31708 --- [           main] o.s.web.servlet.DispatcherServlet        : Initializing Servlet 'dispatcherServlet'
2022-11-04 18:45:29.862  INFO 31708 --- [           main] o.s.web.servlet.DispatcherServlet        : Completed initialization in 1 ms
2022-11-04 18:45:29.880  INFO 31708 --- [           main] o.e.jetty.server.AbstractConnector       : Started ServerConnector@307e4c44{HTTP/1.1, (http/1.1)}{0.0.0.0:6070}
2022-11-04 18:45:29.882  INFO 31708 --- [           main] o.s.b.web.embedded.jetty.JettyWebServer  : Jetty started on port(s) 6070 (http/1.1) with context path '/api/flights/catalog'
2022-11-04 18:45:29.901  INFO 31708 --- [           main] com.twa.flights.api.catalog.App          : Started App in 10.45 seconds (JVM running for 11.481)
2022-11-04 18:45:41.662  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:42.345  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:42.385  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:42.414  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.075  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.156  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.229  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.272  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.351  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.374  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.433  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.508  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.508  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.559  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.559  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.600  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.611  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.659  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.664  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.709  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.714  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.753  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.758  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.807  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.812  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.886  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.891  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.926  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.926  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.954  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:47.954  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.976  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:47.980  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.003  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.015  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.035  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.040  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.054  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.081  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.091  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.111  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.111  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.138  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.138  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.180  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.184  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.205  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.211  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.239  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.246  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.261  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.270  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.300  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.310  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.359  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.359  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.408  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.409  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.453  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.457  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.482  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.485  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.509  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.521  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.559  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.565  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.598  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.600  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.615  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.617  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.639  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.642  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.659  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.662  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.679  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.681  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.696  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.705  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.716  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.739  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.749  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.762  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.786  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.802  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.820  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.845  INFO 31708 --- [tp1933493643-27] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.853  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.875  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.893  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.901  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.928  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.935  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:48.971  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:48.971  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.009  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.011  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.033  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.040  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.058  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.058  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.074  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.080  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.098  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.107  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.134  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.136  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.154  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.161  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.188  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.192  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.221  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.228  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.245  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.304  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.311  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.331  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.353  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.364  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.388  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.406  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.420  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.425  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.439  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.444  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.458  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.469  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.474  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.486  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.497  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.519  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.527  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.549  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.549  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.569  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.574  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.603  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.604  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.624  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.637  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.647  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.657  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.665  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.676  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.679  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.694  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.698  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.708  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.716  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.727  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.732  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.751  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.755  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.772  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.778  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.808  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.821  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.855  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.863  INFO 31708 --- [tp1933493643-26] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.900  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.900  INFO 31708 --- [tp1933493643-31] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.936  INFO 31708 --- [tp1933493643-29] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.939  INFO 31708 --- [tp1933493643-30] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE
2022-11-04 18:45:49.965  INFO 31708 --- [tp1933493643-32] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code MIA
2022-11-04 18:45:49.988  INFO 31708 --- [tp1933493643-25] c.t.f.a.c.controller.CatalogController   : Obtain all the information about the city with code BUE

```
