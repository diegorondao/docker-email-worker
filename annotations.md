# Algumas anotações

Rodar o todo os serviços: `docker-compose up -d`

Escalar os workers: `docker-compose up -d --scale worker=<NUMBER>`

Executar um comando no container com o postgres: `docker-compose exec db psql -U postgres -c '\l'`

Listando os emails inseridos no banco de dados: `docker-compose exec db psql -U postgres -d email_sender -c 'SELECT * FROM emails'`

Parar os serviços: `docker-compose down`

Exibir os logs dos serviços: `docker-compose logs -f -t`
