In the spirit of learning I will be taking and writing down notes from my experience in developing project : [blog](https://github.com/NiksSkersts/blog)  
  
Entry #1        
In an event when you're developing C# Avalonia (possibly applies to other apps) app and you consume a WEB API, and you receive an TLS "ProtocolVersion" error. There is a possibility that Nginx config is incorrect.       
Be Warned: Localhost,Postman and other API testing apps will work normally.

To solve it add or replace "ssl_protocols *" with "ssl_protocols TLSv1.2 TLSv1.3;" in nginx.conf and server conf.       
For further information check out commit:[Fix "ProtocolVersion" Error in C# app.](https://github.com/NiksSkersts/main_server/commit/0d5959eec437d6edc045dfe6d6adee6d810828ca)

Entry #2