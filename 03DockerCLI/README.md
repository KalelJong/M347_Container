#Docker CLI Commands
1. Überprüfen Sie die Docker-Version. Welchen Befehl müssen Sie dafür verwenden?
   - docker --version
2. Suchen Sie nach einem offiziellen Docker-Image (nginx, apache, mysql, ubuntu usw.) auf Docker Hub. Welcher Command ist dafür geeignet?
   - docker pull
3. Laden Sie das ausgewählte Image auf Ihren Computer herunter.
   - docker pull ubuntu
4. Starten Sie einen neuen Container mit dem heruntergeladenen Image. Tipp: Der Parameter "-d" sorgt dafür, dass der Container im Hintergrund läuft.
   - docker run --name some-mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mysql
5. Überprüfen Sie den Status des Containers.
   - docker ps -a
6. Öffnen Sie eine interaktive Shell im Docker-Container. Dieser Befehl sollte eine interaktive Shell innerhalb des Docker-Containers öffnen.
    - docker exec -it my-postgres-container /bin/bash
7. Führen Sie einige Befehle innerhalb des Containers aus, um die Anwendung zu testen. Je nach Anwendung können dies unterschiedliche Befehle sein.
8. Beenden Sie die interaktive Shell im Docker-Container
    - exit
9.  Stoppen Sie den Container
    - docker stop mysqlcontainer 
10. Überprüfen Sie die Liste der gestoppten Container. Stellen Sie sicher, dass der gestoppte Container in der Liste enthalten ist.
    - docker ps -a
11. Entfernen Sie den gestoppten Container.
    - docker rm mysqlcontainer
    