# Kie Live Example

## COMMANDS:

### Start App

```bash
mvn clean package quarkus:dev
```

### Create Users:

```bash
curl -H "Content-Type: application/json" -H "Accept: application/json" -X POST http://localhost:8080/hiring -d @- << EOF
{
  "candidate": {
    "name": "Harry Potter",
    "email":"potter@email.com"
  }
}
EOF
```

```bash
curl -H "Content-Type: application/json" -H "Accept: application/json" -X POST http://localhost:8080/hiring -d @- << EOF
{
  "candidate": {
    "name": "Paulo",
    "email":"paulo@email.com"
  }
}
EOF
```

```bash
curl -H "Content-Type: application/json" -H "Accept: application/json" -X POST http://localhost:8080/hiring -d @- << EOF
{
  "candidate": {
    "name": "Pere",
    "email":"pere@email.com"
  }
}
EOF
```

### Create forms
In the compiled project!

```bash
./form-generation-cli-linux
```

### URLS
* Running app: http://localhost:8080
* Quarkus Dev UI: http://localhost:8080/q/dev
* Forms js: https://pefernan.github.io/formDropdowns.js