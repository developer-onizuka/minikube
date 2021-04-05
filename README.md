```
PS C:\Users\developer> D:
PS D:\>
PS D:\> cd .\k8s\
PS D:\k8s>
PS D:\k8s> ls


    ディレクトリ: D:\k8s


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        2021/04/05     22:29       41442816 kubectl.exe


PS D:\k8s>
PS D:\k8s> minikube start --vm-driver=virtualbox
* Microsoft Windows 10 Pro 10.0.19042 Build 19042 上の minikube v1.18.1
* 設定を元に、 virtualbox ドライバを使用します
* VM ブートイメージをダウンロードしています...
    > minikube-v1.18.0.iso.sha256: 65 B / 65 B [-------------] 100.00% ? p/s 0s
    > minikube-v1.18.0.iso: 212.99 MiB / 212.99 MiB  100.00% 2.63 MiB p/s 1m21s
* コントロールプレーンのノード minikube を minikube 上で起動しています
* Kubernetes v1.20.2 のダウンロードの準備をしています
    > preloaded-images-k8s-v9-v1....: 491.22 MiB / 491.22 MiB  100.00% 2.71 MiB
* virtualbox VM (CPUs=2, Memory=2200MB, Disk=20000MB) を作成しています...
* Docker 20.10.3 で Kubernetes v1.20.2 を準備しています...
  - Generating certificates and keys ...
  - Booting up control plane ...
  - Configuring RBAC rules ...
* Kubernetes コンポーネントを検証しています...
  - Using image gcr.io/k8s-minikube/storage-provisioner:v4
* 有効なアドオン: storage-provisioner, default-storageclass
* Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default
PS D:\k8s> minikube.exe status
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured
timeToStop: Nonexistent

PS D:\k8s> minikube.exe ssh
                         _             _
            _         _ ( )           ( )
  ___ ___  (_)  ___  (_)| |/')  _   _ | |_      __
/' _ ` _ `\| |/' _ `\| || , <  ( ) ( )| '_`\  /'__`\
| ( ) ( ) || || ( ) || || |\`\ | (_) || |_) )(  ___/
(_) (_) (_)(_)(_) (_)(_)(_) (_)`\___/'(_,__/'`\____)

$ docker images
REPOSITORY                                TAG        IMAGE ID       CREATED         SIZE
k8s.gcr.io/kube-proxy                     v1.20.2    43154ddb57a8   2 months ago    118MB
k8s.gcr.io/kube-controller-manager        v1.20.2    a27166429d98   2 months ago    116MB
k8s.gcr.io/kube-apiserver                 v1.20.2    a8c2fdb8bf76   2 months ago    122MB
k8s.gcr.io/kube-scheduler                 v1.20.2    ed2c44fbdd78   2 months ago    46.4MB
kubernetesui/dashboard                    v2.1.0     9a07b5b4bfac   3 months ago    226MB
gcr.io/k8s-minikube/storage-provisioner   v4         85069258b98a   4 months ago    29.7MB
k8s.gcr.io/etcd                           3.4.13-0   0369cf4303ff   7 months ago    253MB
k8s.gcr.io/coredns                        1.7.0      bfe3a36ebd25   9 months ago    45.2MB
kubernetesui/metrics-scraper              v1.0.4     86262685d9ab   12 months ago   36.9MB
k8s.gcr.io/pause                          3.2        80d28bedfe5d   13 months ago   683kB
```
