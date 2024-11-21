# Ducking Traps

1. Problem: error on attempt to consume message using Kafka Rest Proxy
    ```json
    {"error_code":40801,"message":"java.io.CharConversionException: Invalid UTF-32 character..."}
    ```
   _Solution_: change `"format": "json"` to `"format": "jsonschema"` when create a consumer `/consumers/test_consumer_group`