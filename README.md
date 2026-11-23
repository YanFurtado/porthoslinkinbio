# Porthos Barbearia - Link in Bio

## Rodar local
    docker build -t porthos-linkinbio .
    docker run -d --name porthos -p 8080:80 --restart unless-stopped porthos-linkinbio
Abra http://localhost:8080

## Deploy (Coolify / EasyPanel / Portainer)
- Build pack: Dockerfile (na raiz desta pasta)
- Porta do container: 80
- Healthcheck: /healthz
- Domínio + HTTPS: configurar no painel (proxy reverso faz o SSL)

## Atualizar conteúdo
Edite os arquivos em `public/` e faça um novo build/deploy.
