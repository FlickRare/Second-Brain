# Network Programmability Fundamentals

## Programming Fundamentals:
### Data Formats and structured data: machine friendly over human readable
- XML (Extensable Markup language:
    - Pros:  can carry more complex data structures (metadata, etc.
    - Cons: Harder to read and work with for humans.
    ``` xml
    <?xml version="1.0" encoding="UTF-8" ?>
    <addresses>
        <ip>172.16.0.2</ip>
        <netmask>255.255.255.0</netmask>
    </addresses>
    <addresses>
        <ip>172.16.0.3</ip>
        <netmask>255.255.255.0</netmask>
    </addresses>
    <addresses>
        <ip>172.16.0.4</ip>
        <netmask>255.255.255.0</netmask>
    </addresses>
    ```

- JSON (javascript object notation):
    - Pros: a good bit easier to read for humans, more lightweight, indicators for data structure types match python.
    - Cons: Not as many features as XML
    ``` JSON
    {
        "addresses": [
        {
            "ip": "172.16.0.2",
            "netmask": "255.255.255.0"
        },
        {
            "ip": "172.16.0.3",
            "netmask": "255.255.255.0"
        },
        {
            "ip": "172.16.0.4",
            "netmask": "255.255.255.0"
        }
        ]
    }
    ```
- YAML (YAML aint markup langauge):
    - Pro: Easiest to read and most lightweight format
    - Con: Same as JSON
    ``` YAML
    ---
    addresses:
    - ip: 172.16.0.2
        netmask: 255.255.255.0
    - ip: 172.16.0.3
        netmask: 255.255.255.0
    - ip: 172.16.0.4
        netmask: 255.255.255.0
    ```
- What are APIs?:
    - APIs are sets of requirements that govern how one application can talk to another.
    - Main Types:
        - Simple Object Access Protocol (SOAP): Early, powerful but complex and rigged implementation of APIs.
        - RPC vs REST (https://aws.amazon.com/compare/the-difference-between-rpc-and-rest/):
            - RPC APIs allow developers to call remote functions in external servers as if they were local to their software. For example, you can add chat functionality to your application by remotely calling messaging functions on another chat application. 
            - In contrast:
            -  REST APIs allow you to perform specific data operations on a remote server. For example, your application could insert or modify employee data on a remote server by using REST APIs.
