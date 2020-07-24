sudo docker-compose up -d  
sudo docker-compose ps  
sudo docker-compose exec db psql -U postgres -c '\l'  
sudo docker-compose down  

sudo docker-compose exec db psql -U postgres -f /scripts/check.sql  

sudo docker-compose logs -f -t  

sudo docker-compose up -d --scale worker=3  

