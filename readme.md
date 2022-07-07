# MyChat

## Description 
Um sistema de videoconferência direcionado para a comunicação entre funcionários da CME.

##  How to use this source code

#### 1 - Clone repo
```
git clone https://github.com/divanov11/mychat
```

#### 2 - Install requirements
```
cd mychat
pip install -r requirements.txt
```

#### 3 - Update Agora credentals
De forma a ser utilizada por terceiros, é necessário trocar as credencias da api agora nos ficheiros `views.py` e `streams.js`.

Criar uma conta em agora.io, criar uma `app`. Posteriormente, copiar `appid` e `appCertificate` para atualizar em `views.py` e `streams.js`.

###### views.py
```
def getToken(request):
    appId = "TEU APP ID"
    appCertificate = "TEU APPS CERTIFICATE"
    ......
```

###### streams.js
```
....
const APP_ID = 'TEU APP ID'
....
```


#### 4 - Iniciar o programa
```
python manage.py runserver
```


