1. Zainstalujcie vagrant-a lokalnie
2. Sklonujcie to repo: https://github.com/JacekMajchrzak/cd-workshops
3. wejdzcie do głównego katalogu repo i odpalcie vagrant up - powienien postawic Wam dwa wirtual boxy: jenkins i dev
4. Użyjcie komenty vagrant ssh jenkins zeby wejść na box jenkinsa i odpalcie tam:   docker run -d -u root -p 8081:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock visibilityspots/jenkins-docker
5. docker ps  (odczytajcie id jenkinsa, wystarczy pierwsze pare znaków)
6. docker logs <id>  - znajdzcie w logach hasło do jenkinsa, powinno znaleźć się na dole
7. Otwórzcie w przeglądarce  10.0.0.200:8081
8. Wprowadźcie hasło znalezione wcześniej w logach
9. Zainstalujcie sugerowane pluginy
10. Wprowadźcie credentiale admin i wciśnijcie save and continue
11. Save and finish
Macie działający jenkins którego użyjemy w trakcie warsztatów
