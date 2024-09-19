# HAProxy docker compose
This is a simple docker compose file to run HAProxy in a container with a simple web server (jmalloc/echo-server) as the backend.

## Usage
1. Clone the repository
2. Run `docker compose up -d`
    - `docker compose logs -f` to see the logs
3. Access HAProxy stats at [http://localhost:8404](http://localhost:8404)
4. Access web (jmalloc/echo-server) at [http://localhost](http://localhost)


## Vagrant
You can also use Vagrant (Debian) to run HAProxy and the web server. 

Adjust the **config.vm.network** network adapter to your needs in the **vagrantfile**<br> 
I use tested this with my primary network adapter.

Just run `vagrant up` and access:
-  HAProxy stats at [http://localhost:8404](http://localhost:8404)
- and the web server at [http://localhost:8080](http://localhost:8080)