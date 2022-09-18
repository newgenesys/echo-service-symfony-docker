# Technical Requirements

- PHP 8.1+
- Composer

# Setup

1. Clone the repository `git clone git@github.com:lend-invest/echo-service.git`
2. Navigate to the repository's folder `cd echo-service`
3. Install composer's packages `composer install`

# Available routes
  - /healthcheck
  - /echo

# Example requests
 
#### /healthcheck
```
curl --request GET \
  --url http://127.0.0.1:8000/healthcheck \
  --header 'Content-Type: application/json'
```
  
#### /echo
```
curl --request POST \
  --url http://127.0.0.1:8000/echo \
  --header 'Content-Type: application/json' \
  --data '{
	"message": "put your message here"
}'
```
