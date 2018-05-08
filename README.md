# Aprendendo-Cordova
guias, tutoriais e etcs
#
### Comando do cordova.
- Criar estrutura do aplicativo: ``` Cordova create <nome do projeto>```
- Adicionando plugin ao aplicativo: ``` cordova plugin add <nome do plugin> ``` obs: Lembre de configurar o plugin no arquivo index.js
- Listando plugins do aplicativo: ```cordova plugin ls```
- Removendo plugins do aplicaativo: ```cordova plugin rm nome-do-plugin```
- Adicionado plataforma: ```cordova platform add android```

| Plataforma | Comando |
| ------ | ------ |
| android | cordova platform add android|
| ios | cordova platform add ios|
| browser | cordova platform add browser  |
| osx | cordova platform add osx |

- Gerando app via build:  ```cordova build <nome da plataforma>``` 

- Testando aplicativo: ```cordova run android``` obs: tesntando dessa forma vc precisa ativar a ```opção de desenvolvedor``` do android e também conectar o celular ao computador com o cabo ```USB``` 


#

### (PARA-ANDROID-IOS)  Utilizando plugins no cordova.
No cordova podemos adicionar plugins para torna o desenvolvimento mais rápido. Hoje vamos aprender a como adiciona, lista e remover plugins.

Podemos encontrar os plugins do cordova no site: https://cordova.apache.org/plugins/ 

1-	Abra o terminal, e vá até a pasta do projeto.

2-	Para adicionar um plugin no projeto e só utilizar o comando ```cordova plugin add nome-do-plugin```. 

3-	Com o plugin baixado, agora vamos configurar a extensão no arquivo ```js/index.js```. Cada plugin tem um manual na pagina de como configurar, agora e só seguir o manual de cada um. 

4-	 Para listar os plugins de uma aplicação utilizamos o comando ```cordova plugin ls```

5-	Para remover um plugin de uma aplicação utilizamos o comando ```cordova plugin rm nome-do-plugin```



#
#### (PARA-ANDROID) Adicionando icone a aplicação cordova.

1- Procure o arquivo config.xml na pasta da aplicação e abra.

2- no final do arquivo antes da teg ``` '</widget>'``` adicione o trecho de código.

```
  
<platform name="android"> <!--apenas para aplicação android--> 
        <!--
            ldpi    : 36x36 px - ldpi (baixa) ~ 120 dpi <!--dimensão de icone para tela com densidade ldpi-->
            mdpi    : 48x48 px - mdpi (média) ~ 160 dpi <!--dimensão de icone para tela com densidade mdpi-->
            hdpi    : 72x72 px - hdpi (alta) ~ 240 dpi <!--dimensão de icone para tela com densidade hdpi-->
            xhdpi   : 96x96 px - xhdpi (extra-alta) ~ 320 dpi <!--dimensão de icone para tela com densidade xdpi-->
            xxhdpi  : 144x144 px - xxhdpi (extra-extra-alta) ~ 480 dpi <!--dimensão de icone para tela com densidade xxldpi-->
            xxxhdpi : 192x192 px - xxxhdpi (extra-extra-extra-alta) ~ 640 dpi <!--dimensão de icone para tela com densidade xxxldpi-->
        -->
        <icon src="res/android/ldpi.png" density="ldpi" /> <!--nomes corretos para os icones 36x36 -->
        <icon src="res/android/mdpi.png" density="mdpi" /> <!--nomes corretos para os icones 48x48 -->
        <icon src="res/android/hdpi.png" density="hdpi" /> <!--nomes corretos para os icones 72x72 -->
        <icon src="res/android/xhdpi.png" density="xhdpi" /> <!--nomes corretos para os icones 96x96 -->
        <icon src="res/android/xxhdpi.png" density="xxhdpi" /> <!--nomes corretos para os icones 144x144 -->
        <icon src="res/android/xxxhdpi.png" density="xxxhdpi" /> <!--nomes corretos para os icones 192x192 -->
</platform>
```
3- Va na pasta ```res/android/ ``` e adicione os icones. Lembrando que segue como e informado no código.

 - O icone de 36x36 pixel tem que ter o nome ldpi.png
 - O icone de 48x48 pixel tem que ter o nome mdpi.png
 - O icone de 72x72 pixel tem que ter o nome hdpi.png
 - O icone de 96x96 pixel tem que ter o nome xhdpi.png
 - O icone de 144x144 pixel tem que ter o nome xxhdpi.png
 - O icone de 192x192 pixel tem que ter o nome xxxhdpi.png
 
 4- Agora e só gerar o app.
 #
 
 #### (PARA-ANDROID)  Criando splash
 
 
