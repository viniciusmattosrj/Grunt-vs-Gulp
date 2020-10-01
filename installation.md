# Instalação

Faça um git clone do projeto node:
```
git clone git@github.com:viniciusmattosrj/grunt-vs-gulp.git
```

## Encoding

Todos os arquivos estão em **UTF-8**.


#### Importante para que o git não considere alterações de permissão como modificações a serem rastreadas

```
git config core.fileMode false
```

#### Usando o nvm

No projeto **grunt-vs-gulp** execute o comando abaixo:
```
npm install
```

#### Utilizando o docker ao invés do NVM

Caso você utilize docker ao invés do NVM será necessário realizar a cópia do arquivo example:
```
cp -v docker-compose.yml.example docker-compose.yml
```

Dentro do projeto **grunt-vs-gulp** execute:
```
docker-compose up -d
```

Instalando as dependências do projeto:
```
docker exec -it node bash -c "npm install"
```

#### Somente em ambiente de dev deve ser concedido a permissão nas pastas:

```
sudo chmod 777 -R keys node_modules
```