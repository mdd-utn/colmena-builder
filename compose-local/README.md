cd /mnt/work/workspaces/workspace_antlr/colmena-builder/compose-local

docker-compose up -d


docker-compose up -d --build


 curl -L https://downloads.portainer.io/portainer-agent-stack.yml -o portainer-agent-stack.yml
$ docker stack deploy --compose-file=portainer-agent-stack.yml portainer
