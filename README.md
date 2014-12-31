# openjdk-centos

A `Dockerfile` for creating an OpenJDK image on top of the official CentOS distribution (`centos:latest`).

Multiple tag exist for different versions of OpenJDK:

- `1.7.0-jre` to build OpenJDK version 1.7 with JRE only

## How to Build

    git clone https://github.com/kadishmal/openjdk-centos.git
    cd openjdk-centos
    docker built -t lighthopper/openjdk-centos:1.7.0-jre .

## How to Reuse

In your `Dockerfile` at the very top specify:

    FROM lighthopper/openjdk-centos:<tag>

Replace `<tag>` with any of the available tags.

## License

MIT