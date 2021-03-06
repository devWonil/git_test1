# HTTPS 란



HTTP의 응답과 요청은 평문으로 전달됩니다. 만약 누군가 이를 가로챈다면 중요한 정보가 유출될 수 있습니다. 예를 들어, 로그인할 때 전송한 POST 요청에는 대개 이용자의 ID와 비밀번호가 포함됩니다. 공격자가 중간에 이를 가로채면 이용자의 계정이 탈취당할 수 있습니다.

HTTPS(HTTP over Secure socket layer)는 TLS(Transport Layer Security) 프로토콜을 도입하여 이런 문제점을 보완합니다. TLS는 서버와 클라이언트 사이에 오가는 모든 HTTP 메시지를 암호화합니다. 공격자가 중간에 메시지를 탈취하더라도 이를 해석하는 것은 불가능하며, 결과적으로 HTTP 통신이 도청과 변조로부터 보호됩니다.


HTTPS가 제정된 초기에는 금융이나 정부 서비스와 같이 민감한 데이터를 취급하는 웹 서비스들 위주로 HTTPS가 사용되었습니다. 그러나 현재 개발되는 서비스들은 규모에 상관없이 HTTPS를 사용하는 추세입니다.

웹 서버의 URL이 http://로 시작되면 HTTP, https://로 시작되면 HTTPS 프로토콜을 사용합니다. 





 

![img](https://blog.kakaocdn.net/dn/Kc4zc/btrAxHEDFCy/gfSqKJUwySc3VjYUuPKbG0/img.png)







![img](https://blog.kakaocdn.net/dn/cDPplS/btrAs8X1tii/0lTdckcf7Hte9jndMIn6jk/img.png)







### **정리** 

 

> **HTTP(HyperText Transfer Protocol): 웹 서버와 클라이언트가 리소스를 교환하기 위해 사용하는 프로토콜. 클라이언트가 요청하면, 서버가 응답하는 방식.**
>
> **HTTP 메시지: HTTP 서버와 클라이언트가 교환하는 데이터. 헤드와 바디로 구성되며, 각 줄은 CRLF로 구분됨.**
>
> **헤드: 메시지에 대한 정보. 헤드의 끝에는 CRLF가 한 줄 있음.**
>
> **바디: 클라이언트가 서버에게, 또는 서버가 클라이언트에게 전달할 데이터**
>
> **HTTP 요청(Request): 클라이언트가 서버에게 특정 동작을 요청하는 메시지**
>
> **메소드(Method): 요청 URI가 가리키는 리소스에 대해, 서버가 수행했으면 하는 동작을 지정**
>
> **요청 URI(Request-URI): 메소드의 대상이 되는 리소스를 지정**
>
> **HTTP 응답(Response): 요청을 처리한 결과 및 이유, 그리고 클라이언트에 전송할 웹 리소스를 포함하는 메시지**
>
> **상태 코드(Status Code): 요청을 처리한 결과**
>
> **처리 사유(Reason Phrase): 상태 코드가 발생한 이유**
>
> **HTTPS(HTTP on Secure socket layer): TLS를 이용하여 HTTP의 약점을 보완한 프로토콜**

 

