echo quit | openssl s_client -showcerts -servername server -connect server:443 > cacert.pem
