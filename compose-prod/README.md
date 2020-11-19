cd /mnt/work/workspaces/workspace_antlr/colmena-builder/compose-prod

echo mddutn2020 | docker login  --username mddutn --password-stdin

docker-compose up -d
