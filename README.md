# docker-kubernetes-configs-
Bu depo, Docker ve Kubernetes ortamlarında kullanılmak üzere hazırlanmış yapılandırma dosyalarını içermektedir. Docker Compose, Kubernetes Deployment, Service, HPA ve Prometheus yapılandırmaları mevcuttur.

İçerik

1. Docker

Dockerfile: Özel bir Docker imajı oluşturmak için gerekli talimatları içerir.

compose.yaml: Docker Compose ile çoklu konteyner çalıştırmak için kullanılır.

2. Kubernetes

pod.yaml: Tek bir pod oluşturmak için Kubernetes manifest dosyası.

nodejs-deployment.yaml: Node.js uygulaması için Deployment tanımı.

service.yaml: Kubernetes Service yapılandırması.

hpa.yaml: Horizontal Pod Autoscaler (HPA) yapılandırma dosyası.

metrics.yaml: Kubernetes metriklerini ayarlamak için kullanılır.

3. Prometheus

prometheus.yml: Prometheus izleme yapılandırma dosyası.

Kullanım

Docker Kullanımı

Docker imajını oluşturun:

docker build -t my-app .

Docker Compose ile çalıştırın:

docker-compose up -d

Kubernetes Kullanımı

Pod oluşturun:

kubectl apply -f pod.yaml

Deployment ve Servisleri çalıştırın:

kubectl apply -f nodejs-deployment.yaml
kubectl apply -f service.yaml

HPA yapılandırmasını uygulayın:

kubectl apply -f hpa.yaml

Prometheus Kullanımı

Prometheus'u başlatın:

prometheus --config.file=prometheus.yml

Repository Bilgileri

Repository Adı: docker-kubernetes-configs

Açıklama:
Docker ve Kubernetes ortamlarında kullanılmak üzere hazırlanmış yapılandırma dosyaları. Docker Compose, Kubernetes Deployment, Service, HPA ve Prometheus yapılandırmaları içerir.

Katkıda Bulunma

Eğer geliştirme yapmak isterseniz, lütfen bir "pull request" oluşturun veya yeni bir "issue" açın.

Lisans

Bu proje açık kaynak olup MIT Lisansı ile lisanslanmıştır.
