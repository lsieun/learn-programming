# Http Client

基于Http协议的Client，主要就是围绕request和response进行展开。

- request
    - url
    - headers
    - data:
        - method get
            - query string(param)
        - method post
            - form
                - string
                - file
            - json
            - binary
- response
    - status code
    - header
    - data
        - binary encoding
            - html
            - json
            - text
        - binary not encoding
            - file(内存可以装下的二进制数据))
            - stream(big big file，内存装不下，或者不适合内存存放的数据)

- proxy
- session