# Create a ConfigMap named 'game-config' from a directory
kubectl create configmap game-config --from-file=configure-pod-container/configmap/

# Describe the created ConfigMap for details
kubectl describe configmaps game-config

# Create a ConfigMap named 'game-config-2' from a specific file
kubectl create configmap game-config-2 --from-file=configure-pod-container/configmap/game.properties

# Create a ConfigMap named 'game-config-2' from multiple files
kubectl create configmap game-config-2 \
    --from-file=configure-pod-container/configmap/game.properties \
    --from-file=configure-pod-container/configmap/ui.properties

# Create a ConfigMap named 'game-config-env-file' from an environment file
kubectl create configmap game-config-env-file \
    --from-env-file=configure-pod-container/configmap/game-env-file.properties

# Create a ConfigMap named 'config-multi-env-files' from multiple environment files
kubectl create configmap config-multi-env-files \
    --from-env-file=configure-pod-container/configmap/game-env-file.properties \
    --from-env-file=configure-pod-container/configmap/ui-env-file.properties

# Create a ConfigMap named 'game-config-3' with a specific key from a file
kubectl create configmap game-config-3 --from-file=game-special-key=configure-pod-container/configmap/game.properties

# Create a ConfigMap named 'special-config' from literal values
kubectl create configmap special-config \
    --from-literal=special.how=very \
    --from-literal=special.type=charm

## You can't use ConfigMaps for static pods, because the kubelet does not support this.

