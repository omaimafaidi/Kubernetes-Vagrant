# Astuce : Pour utiliser k à la place de kubectl 
taper sur votre Terminal :

source <(kubectl completion bash) \
echo "source <(kubectl completion bash)" >> ~/.bashrc \
alias k=kubectl \
complete -o default -F __start_kubectl k

