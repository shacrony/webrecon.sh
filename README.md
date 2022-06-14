# webrecon.sh
#!/bin/bash
for palavra in $(cat path wordlist)
do
response=$(curl -s -H "User-Agent: Mozilla/5.0") -o /dev/null -w "%{htttp_code}" $1/$palavra/)
if [$resposta == "200"]
then
echo "Diretorio encontrado: $1/$palavra"
fi
done

legendas:

-H pode ser qualquer user agent não necessariamente mozzila
-o pode ser uma saída pra qualquer outro lugar

usage:

git clone https://github.com/shacrony/webrecon.sh.git

chmod +x 

./webrecon.sh http://sitealvo.com.br

![image](https://user-images.githubusercontent.com/61089592/173628940-9516fc06-de63-4168-b878-78184cfbf586.png)
