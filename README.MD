# Instruções
• Clone o repositório do emulador dentro da pasta server. A pasta com os arquivos do emulador deve se chamar emulador.
• Copie os arquivos com as tabelas sql que deseja importar para db/sql-files.

# Comandos do Docker
• docker-compose -f "docker-compose.yaml" up -d --build
• docker exec -i -t <ID DA IMAGEM> /bin/bash

# Configurações
• conf/import/char_conf.txt
char_ip: 127.0.0.1

• conf/import/map_conf.txt
map_ip: 127.0.0.1

Nota: Não sei o motivo, mas esses 2 ips precisam ser alterados para localhost (127.0.0.1) ou o client não conseguirá se conectar ao server.

• conf/import/inter_conf.txt
login_server_ip: db
ipban_db_ip: db
char_server_ip: db
map_server_ip: db
log_db_ip: db

Nota: 'db' é o nome do host do phpmyadmin. Variável PMA_HOST, arquivo docker-compose.yaml, seção phpmyadmin.