## Shopify Docker Environment Setup to support Headless StoreFront

### Docker Container Setup

#### Create and Start a Docker Container

```bash
docker run --name shopify -id alpine:3.20.1
```

#### Access the Docker Container

```bash
docker exec -it shopify /bin/sh
```

### Inside the Docker Container

#### Install Bash, Git, Node.js, and Ruby

```bash
apk add --no-cache bash git nodejs npm ruby
```

#### Install Bundler (Ruby Gem)

```bash
gem install bundler
```

#### Install Shopify CLI

```bash
npm install -g @shopify/cli@latest
```

### Visual Studio Code Integration

#### Remote Containers Extension

Install the "Remote - Containers" extension in Visual Studio Code:

- Extension: [ms-vscode-remote.remote-containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)


### Shopify Developer

#### Reference Headless

- Guide self-hosting : [https://shopify.dev/docs/storefronts/headless/hydrogen/deployments/self-hosting)


