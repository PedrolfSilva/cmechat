# MyChat

## Descrição
Um sistema de videoconferência direcionado para a comunicação entre funcionários da CME.

##  Como utilizar

#### 1 - Clone repo
```
git clone https://github.com/divanov11/mychat
```

#### 2 - Instalar requerimentos
```
cd mychat
pip install -r requirements.txt
```

#### 3 - Atualizar cerdenciais da Agora
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


