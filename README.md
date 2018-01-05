# Sentiment-Analysis-Keras-Flask
A simple web service to predict Sentiment using CNN.



API USAGE:

```
curl -i -H "Content-Type: application/json" -X POST -d '{"review":"This movies is good"}' http://localhost:5000/review
```


```
HTTP/1.0 200 OK
Content-Type: application/json
Content-Length: 33
Server: Werkzeug/0.11.15 Python/3.6.1
Date: Fri, 05 Jan 2018 23:38:14 GMT

{
  "sentiment   ": "positive"
}
```


```
curl -i -H "Content-Type: application/json" -X POST -d '{"review":"This movies is bad"}' http://localhost:5000/review
```


```
HTTP/1.0 200 OK
Content-Type: application/json
Content-Length: 33
Server: Werkzeug/0.11.15 Python/3.6.1
Date: Fri, 05 Jan 2018 23:38:53 GMT

{
  "sentiment   ": "negative"
}
```
