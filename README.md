# HexRepro

Repro build hang

```bash
docker volume create --name test_deps

docker run --rm -ti -v test_deps:/proj/deps test mix deps.get

# This often hangs:
docker run --rm -ti -v test_deps:/proj/deps test mix test
```
