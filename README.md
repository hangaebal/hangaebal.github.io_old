# GitHub Page 도메인 연결하기
> [hangaebal.github.io](http://hangaebal.github.io)

<br>

https://help.github.com/articles/setting-up-your-pages-site-repository/  보고 진행했는데 간단히 요약하면

-----


## 1. www.xxx.kr 로 연결 하려면

1) GitHub 쪽 준비
- 리파지토리 루트에 CNAME 라는 이름의 파일을 생성해서 `www.xxx.kr` 라는 내용을 추가

2) DNS 설정
- Type: `CNAME` / NAME: `www` / value: `닉네임.github.io`

    .


-----

## 2. xxx.kr 로 연결 하려면


1) GitHub 쪽 준비  
- 리파지토리 루트에 CNAME 라는 이름의 파일을 생성해서 `xxx.kr` 라는 내용을 추가  
    

2) DNS 
- Type: `A` / NAME: `xxx.kr` / value: `192.30.252.153`  
- Type: `A` / NAME: `xxx.kr` / value: `192.30.252.154` (둘 다 추가)  
    
    
3) (선택사항) 추가로 www.xxx.kr 로도 연결하려면  
- Type: `CNAME` / NAME: `www` / value: `닉네임.github.io` 도 추가하면 됩니다.
    
    

-----

CloudFlare 기준 설정 후 5~10분 이내에 금방 연결 확인되었다
