# Openwebui with traefik and ollama

## Components

### Traefik

Traefik acts as Proxy, does ssl offloading and forwards request to openwebui container

### Openwebui

acts as frontend for ollama

### Ollama

needs to be set up as seperate service on mac os x as Mac Silicone does not support GPU support inside docker easily
otherwise can also be started as docker container

on mac os x with brew installed(https://brew.sh/)
    brew install ollama(follow intstructions to add it to path)
    ollama pull mistral-small:latest
    ollama run mistral-small:latest

