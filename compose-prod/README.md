cd /mnt/work/workspaces/workspace_antlr/colmena-builder/compose-prod

echo XXX | docker login  --username mddutn --password-stdin


docker-compose up -d

docker stop colmena_colmena-audit_1
docker stop colmena_colmena-reverse_1
docker stop colmena_colmena-github-webhook_1

docker restart colmena_proxy_1


docker start colmena_colmena-audit_1
docker start colmena_colmena-reverse_1
docker start colmena_colmena-github-webhook_1

