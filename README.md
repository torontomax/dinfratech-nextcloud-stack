# Nextcloud + OnlyOffice + PostgreSQL Stack

Este repositório contém a configuração Docker Compose para rodar uma instância do **Nextcloud** integrada ao **OnlyOffice**, utilizando **PostgreSQL** como banco de dados. Esta stack foi desenhada para operar atrás de um **Nginx Proxy Manager**.

## 🚀 Tecnologias
* **Nextcloud**: Gestão de arquivos e colaboração.
* **OnlyOffice**: Edição de documentos em tempo real.
* **PostgreSQL 15**: Banco de dados robusto.
* **Docker**: Orquestração simplificada.

## 🛠️ Configuração
O deploy está configurado para o domínio `cloud.seudominio.com.br`. Para utilizar:

1. Certifique-se de que a rede docker `nginx-manager_default` existe.
2. Ajuste as senhas e credenciais de SMTP no arquivo `docker-compose.yml`.
3. Execute `docker-compose up -d`.

## 📌 Notas importantes
* **SSL/TLS**: Recomenda-se o uso de certificados via Nginx Proxy Manager.
* **Websockets**: No Proxy, ative o suporte a Websockets para o funcionamento correto do OnlyOffice.
