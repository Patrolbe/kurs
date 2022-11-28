# INSTALACJA APLIKACJI
## pobranie repozytorium do własnego środowiska za pomoca git pull/git clone <link do repozytorium>
## następnie w terminalu wchodzimy do katalogu backend
cd backend
npm install
## instalujemy npm również w front
cd ..
cd front
npm install
# URUCHAMIANIE
## wejsc do katalogu backend i uruchomic index.js
cd backend

node index.js
## wrócić do katalogu głownego
cd ..
## wejsc do katalogu front i uruchomic serwer
cd front     
gp env VUE_APP_SERVER_URL=$(gp url 3000) && eval $(gp env -e)
npm run serve

## wejsc na wyświetlony link
    http://localhost:8080/

#Uwaga 
od rana miałem problem z push na mojego gitahuba, po długich godzinach stwierdziłem, że ręcznie podmienie pliki. Mam nadzieję, że będę mógł jednak przystąpić do konkursu
