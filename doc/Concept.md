## Вступ: Опис інструментів та їх призначення.

1. minikube implements a local Kubernetes cluster on macOS, Linux, and Windows. minikube's primary goals are to be the best tool for local Kubernetes application development and to support all Kubernetes features that fit.

2. kind is a tool for running local Kubernetes clusters using Docker container “nodes”.
kind was primarily designed for testing Kubernetes itself, but may be used for local development or CI.

3. k3d is a lightweight wrapper to run k3s (Rancher Lab’s minimal Kubernetes distribution) in docker. k3d makes it very easy to create single- and multi-node k3s clusters in docker, e.g. for local development on Kubernetes.

## Характеристики:

| Характеристика | minikube | kind | k3d |
| -------------- | -------- | ---- | --- |
| Supported OS  | macOS, Linux, Windows | macOS, Linux, Windows | Linux |
| Automation | CLI and config files | CLI and config files | CLI |
| Features | Supports additional Kubernetes fuctions. | Simple to use. Community support. | Fast cluster creation. Wide config options |

## Переваги та недоліки
| Інструмент | Переваги | Недоліки |
| ---------- | -------- | -------- |
| minikube | 1. Легко встановити і використовувати для розробки та тестування. 2. Швидке створення локального Kubernetes кластера. | Обмежені можливості масштабування порівняно з реальним кластером. |
| kind | 1. Інтеграція з Docker, що дозволяє ефективно використовувати ресурси. 2. Швидке створення Kubernetes кластера в Docker контейнерах. | Можуть виникнути проблеми з обмеженнями ресурсів Docker при масштабуванні. |
| k3d | 1. Простий у використанні та має гнучкі опції налаштування. 2. Швидке створення Kubernetes кластера в Docker контейнерах. | Можливі проблеми зі стабільністю у складних середовищах. |

## Демонстрація k3d
![k3d demonstration](./tty.gif)
