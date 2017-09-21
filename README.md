# Roelof's `docker-compose`

These are my configurations for my server (OS-level dockers).

## Containers

The configuration creates Docker containers for the following images:

- **Gitlab community edition** (`gitlab` / `gitlab.roelof.io`) with services
  - *SSH* on `0.0.0.0:22`
  - *Web app* on `127.0.0.1:8040`

- **PlantUml server**  (`plantuml` / `plantuml.roelof.io`) without services

- **Fidus Writer** (`latex` / `latex.roelof.io`) with services
  - *Web app* on `127.0.0.1:2040`

All dockers are interlinked via the same network (named `gitlab`). This way
GitLab and Fidus can connect to the PlantUML server using the `plantuml`
hostname.

## Configs

There's an `nginx/` directory containing the configurations for nginx. These
are the bare `server`-configs and don't contain tweaking concerning the HTTPS
connections.

SSL-certificate paths are forged (duh)

## License

The project is licensed under the [GNU General Public License 3.0][license].

[license]: LICENSE.md
