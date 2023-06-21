<!-- GETTING STARTED -->
## Getting Started
Remeber that you have to manually run 

* Docker installer
  ```sh
  sh get-docker.sh
  ```
* Portainer installer
  ```sh
  docker volume create portainer_data
  docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest
  ```

* MySQL config
  ```sh
  dpkg -i mysql-apt-config*
  ```