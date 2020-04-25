# shikanga-concourse-workshops
Concourse-CI Related Workshops

## Quick Start
Concourse is distributed as a single concourse binary, making it easy to run just about anywhere, especially with Docker.

```
$ wget https://concourse-ci.org/docker-compose.yml
$ docker-compose up -d
```
Concourse will be running at `localhost:8080.` You can log in with the username/password as `test/test.`

Next, install [fly CLI](https://concourse-ci.org) by downloading it from the web UI.

Click on your operating system to download the fly CLI.

Once downloaded, copy the fly binary into your path ($PATH), such as `/usr/local/bin` or `~/bin.` Don't forget to also make it executable. For example:

```
sudo mkdir -p /usr/local/bin
sudo mv ~/Downloads/fly /usr/local/bin
sudo chmod 0755 /usr/local/bin/fly
```

Test your fly CLI installation by displaying the version installed i.e.
```
$ fly -v
```

Target your local Concourse as the `test` user:

```
$ fly -t tutorial login -c http://localhost:8080 -u test -p test
```

Once set up, the tutorials in the following website should get you familiar with concourse-ci [concoursetutorial.com](https://concoursetutorial.com)
