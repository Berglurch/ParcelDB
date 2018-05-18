# ci_cd-database

Buildbefehl:
docker build -t parcel-db .

Startbefehl:  
Falls schon eine MySQL-Instanz auf dem Hostsystem läuft, muss auf einen anderen Port weitergeleitet werden

docker run -d --restart always --network=parcelnetwork -p 3306:3306 --name=parcel-db parcel-db
