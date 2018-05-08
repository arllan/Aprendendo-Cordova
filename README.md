# Aprendendo-Cordova
guias, tutoriais e etcs
#
#### (PARA-ANDROID) Adicionando icone a aplicação cordova.

1- Procure o arquivo config.xml na pasta da aplicação e abra.

2- no final do arquivo antes da teg ``` '</widget>'``` adicione o trecho de código.

```sh
  
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
 
 
