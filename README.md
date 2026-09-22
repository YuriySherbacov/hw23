cat > /mnt/c/Users/alina/Desktop/homework/hw23/README.md << 'EOF'
# HW23: nginx Pod + Service (kind)

Локальний кластер kind, Pod з nginx, Service типу NodePort (порт 80 → 30080).

## Файли
- `kind-config.yaml` — створення кластера
- `nginx.yaml` — Pod і Service

## Запуск
```bash
kind create cluster --config kind-config.yaml
kubectl apply -f nginx.yaml