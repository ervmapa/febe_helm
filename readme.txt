helm install testa .
helm delete testa

mats@master:~/yamls/febeapp/mychart$  curl -X POST -H "Content-Type: application/json" -d '{"type": "create", "user": "spelle", "data": "helloxxxx"}' http://localhost:30878/control
{"message":"Backend request processed successfully"}

mats@master:~/yamls/febeapp/mychart$  curl -X POST -H "Content-Type: application/json" -d '{"type": "delete", "user":
 "spelle", "data": "helloxxxx"}' http://localhost:30878/control
{"message":"Backend request processed successfully"}
