---
notion-id: 35f96a3c612780adb484f457ac72fd72
Status: Not started
Type: Assessment
---
ss -a

  

  

  

  

![[image.png]]

0010 - 16바이트

  

Type - 다음 레이어 정보

  

세션 생성 → 자원 소모

  

layer4 segment → MSS + MTU

  

stop&wait 방식 / pipeline 방식

  

pipeline 방식 - 선행조건: 수신 버퍼가 충분해야한다, 순서번호가 커져야 한다

- GBN(go-back-n)
- SR(select&repeat)

  

  

stop&wait 방식

  

  

IPv4 32bit(4byte)

192.168.0.0

x.x.x.y

x= 네트워크 주소

y= 호스트 주소 → 254개( 2^8 )까지 가능함

넷마스크 255.255.255.0 통한 앤드연산

192.168.86.2 → 192.168.86.0

  

  

no shut down

ip route NETWORK주소 넷마스크

  

show ip interface brief

show running-config

  

  

  

A클래스 기준 대한민국 4개 가능

  

192.168.86.0

총 호스트 개수 0~256

사용 가능한 호스트 개수 1~254

0 = 네트워크 대역 이름

256 = 브로드캐스트주소

  

  

4등분

0~64

넷웤 0 , 64 , 128 , 192

호스트 1~ 62 , 65~ 126 , 129 ~ 190 , 193 ~ 254

브로드캐스트 63 , 127 , 191 , 255

255.255.255.192

IP 주소 /26