# FreeUnit Documentation

[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
[![GitHub Discussions](https://img.shields.io/badge/GitHub-discussions-009639)](https://github.com/freeunitorg/freeunit/discussions "GitHub Discussions")

Source for the [FreeUnit](https://freeunit.org/) documentation website, written in
[reStructuredText](https://en.wikipedia.org/wiki/ReStructuredText) and built
with [Sphinx](https://www.sphinx-doc.org/en/master/).

FreeUnit is a community-maintained fork of the NGINX Unit application server
(archived October 2025).

## Development

```shell
git clone https://github.com/freeunitorg/docs && cd docs
pip install -r requirements.txt
make serve
```

## Docker (local)
```shell
docker stop freeunit-docs; docker rm freeunit-docs 2>/dev/null; docker build -f Dockerfile.local -t freeunit-docs-local . && docker run -d -p 8000:8000 --name freeunit-docs freeunit-docs-local
http://localhost:8000/
```



The site is served locally at `http://localhost:8000`.

Pull requests automatically deploy a preview site when opened by a maintainer.

## Contributing

Pull requests are welcome. For major changes, please open an issue first.

- **Discussions:** [github.com/freeunitorg/freeunit/discussions](https://github.com/freeunitorg/freeunit/discussions)
- **Security:** [team@freeunit.org](mailto:team@freeunit.org)

## License

The FreeUnit documentation is licensed under [CC BY 4.0](LICENSE).

---

*Forked from [nginx/unit-docs](https://github.com/nginx/unit-docs) — original authors retain full credit.*
