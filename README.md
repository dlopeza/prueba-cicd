<h1>Prueba cd CI/CD con GitHub Actions</h1>
Buildea la imagen luego de cada push, y realiza el deploy en un cluster Kubernetes.
<h2>Configuración en Github</h2>
Setear en <b>Settings->Secrets</b> las variables para la conexión con DockerHub:
<li>DOCKER_USER: usuario de Dockerhub</li>
<li>DOCKER_PASSWORD: password de Dockerhub</li>
<li>DOCKER_REPO: repositorio de Dockerhub</li>
<li>KUBE_CONFIG_DATA: archivo kubeconfig encodeado en base64. </br> En linux se puede hacer con <code>cat $HOME/.kube/config | base64</code></li>
