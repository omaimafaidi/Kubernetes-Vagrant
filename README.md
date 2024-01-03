 # Monter un cluster Kubernetes avec vagrant et virtualbox (un master et un worker)
Taper: git clone https://github.com/grassanordine/kubernetes-certification-stack.git \
cd kubernetes-certification-stack \
Lancer: vagrant up \
Après install lancer: vagrant ssh master \
Si ça marche pas taper:  ssh -p <N°port> vagrant@127.0.0.1 \ 
mot de passe : vagrant \
Rq : (regardez plus haut généralement N° de port: 2222) 

Travailler dans le master avec l'utilisateur root lancer: sudo su \ 
puis taper : kubectl get nodes \

NB : (si toutefois le worker n'est pas monté (notReady) ) taper : vagrant up worker1 \
(dans un autre terminal bien entendu) 

# Astuce : Pour utiliser k à la place de kubectl 
taper sur votre Terminal :\
source <(kubectl completion bash) \
echo "source <(kubectl completion bash)" >> ~/.bashrc \
alias k=kubectl \
complete -o default -F __start_kubectl k

